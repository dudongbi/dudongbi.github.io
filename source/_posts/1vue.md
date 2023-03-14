---
title: 1vue
date: 2022-12-27 11:25:08
tags: [vue]
---

# windows

```bash
get-ExecutionPolicy
set-ExecutionPolicy RemoteSigned
```

注册表
```
[HKEY_CLASSES_ROOT\.ts] 改为 .ts1
[HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Explorer\Kindmap].ts="document"
```

# vite.js

## `package.json`
```json
"build": "vue-tsc --noEmit --skipLibCheck && vite build",
"build1": "vue-tsc --noEmit --skipLibCheck && node --max_old_space_size=16384 ./node_modules/vite/bin/vite.js build",
```

## `tsconfig.json`
```ts
"exclude": ["src/-server/**"], // 排除后端
```

## `vite.config.js`

```ts
import { defineConfig } from 'vite'
import vue from '@vitejs/plugin-vue'

import { resolve } from 'path'
import { viteMockServe } from 'vite-plugin-mock'
import ElementPlus from 'unplugin-element-plus/vite'
// import ViteComponents from 'unplugin-vue-components/vite'
// import { ElementPlusResolver } from 'unplugin-vue-components/resolvers'
// ViteComponents({ resolvers: [ElementPlusResolver()] }),

// https://vitejs.dev/config/
// [style -> template]
//     <style> :export { varSideBarWidth: mystyle.$sideBarWidth; } </style>
//     <template> <component :width="$style.varSideBarWidth" /> </template>
// [script -> style]
//     <script> const color = ref(0xffffff) </script>
//     <style> .div { background-color: v-bind(color) } </style>
export default defineConfig({
    plugins: [ vue(), ElementPlus({useSource: true}), viteMockServe({mockPath:'src/mock'}) ],
    //! tsconfig.json 同步增加 "baseUrl": ".", "paths": { "@/*": ["src/*"] },
    resolve: { alias: { '@': resolve(__dirname, 'src'),  'vue-i18n': 'vue-i18n/dist/vue-i18n.cjs.js' } },
    // [docs] https://mattferderer.com/use-sass-variables-in-typescript-and-javascript
    css: { preprocessorOptions: { scss: { additionalData: `@use "@/mystyle.scss" as mystyle;` } } }
})
```

## `env.d.ts`
```ts
declare module '*.geojson' { // 支持文件
    const value: string;
    export default value;
}
// https://www.jianshu.com/p/783c17fdeb1e # d.ts使用import
declare module 'bpmn-js-properties-panel/PropertiesPanel.js' {
    import { Class, Constructor } from "type-fest";
    interface IModelerConstructorArguments {
        configuration?: Object,
        /* ... */
        createChild: (modules: Array<any>, forceNewInstances: Class<IDidiInjector>) => Constructor<IDidiInjector>,
    }
    export default class Modeler {
        constructor(args: IModelerConstructorArguments);
        attachTo: (parentNode: HTMLElement) => void;
    }
    ...
}

/// <reference path = "./bpmn.d.ts" />
import PanelProperties from 'bpmn-js-properties-panel/index.js';
```

## `@/App.vue`

```ts
<style lang="scss">
html, body, #app {
    padding: 0px;
    margin: 0px;
    height: 100%;
}
</style>
<style scoped lang="scss">
.el-main {
    padding: 0 !important; // 去除 el-main 自带的 --el-main-padding
    height: 100vh;
}
</style>
```

## `mystyle.scss`
```ts
@mixin threejs_container(){
    padding: 0px;
    margin: 0px;
    width: 100%;
    height: 100%;
    box-sizing: border-box;
    border-width: 2pt; // <50
    border-style: solid;
    border-color: red;
}

// TO USE:
<style scoped lang="scss">
.container {
    @include mystyle.threejs_container();
}
</style>
```

# VUE

## 禁止报错
```ts
//@ts-ignore
```

## 引入字符串
```ts
import fragmentShader from './fragmentShader.frag?raw';
```

## 双向绑定
```ts
const emits = defineEmits<{(e:'modelValue'): void}>()
props({ modelValue })
emits('update:modelValue')
```

## 类型
```ts
const cartGrouped: Ref<ICartGrouped> = ref([]); // 是正确
const cartGrouped = ref<ICartGrouped>([]); // 是错误
```

## 键类型
```ts
type IKeyOfX = [key in keyof X]?: X[]
locale as keyof typeof localeOptions
const { locale } = storeToRefs(useSettingStore())
```

## css使用ts
```css
$width: v-bind(width)
```

## html使用css
```html
<div width="$style.sideBarWidth">
```
```css
:export { sideBarWidth: mystyle.$sideBarWidth }
```

# THREE.js

## 几种线

`Curve` → `CurvePath` → `Path`

`getPoints(d)`基于`getPoint`获得d+1个点

`getSpacedPoints(d)`基于`getPointAt`获得d+1个点

`getPoint`按照变量 --vs-- `getPointAt`按照弧长

连续多点：

`Line` 折线

`LineLoop` 闭合折现

`SplineCurve` 平滑二位曲线

`CatmullRomCurve3` 平滑三维曲线

两点：

`LineSegments` 线段（也可以是多个线段，但为偶数点）

`LineCurve3` 曲线

`QuadraticBezierCurve3` 三维二次贝塞尔曲线（一个控制点）

`CubicBezierCurve3` 三维三次贝塞尔曲线（两个控制点）

## BufferGeometry 的四种用法

星云`Points`（在`geometry`指定`size`的版本），见`globe/EarthParticles`
```ts
const geometry = new THREE.BufferGeometry()
const pos = Float32Array.from( (VectorTuple3[]).flat() )
geometry.attributes.position = new THREE.BufferAttribute(pos, 3)
const size = Float32Array.from( number[] )
new THREE.Points(geometry, data[i].material)
```

星云`Points`（在`material`指定`size`的版本），见`globe/satellite`
```ts
const geometry = new THREE.BufferGeometry().setFromPoints( Vector3[] )
const material = new THREE.PointsMaterial({ size: 1, })
new THREE.Points( geometry, material );
```

飞线`Points`（在`fragment`指定`size`的版本），见`globe/outline`
```ts
const geometry = new THREE.BufferGeometry().setFromPoints( Vector3[] );
const percents = new Float32Array( Vector3[].map(_,i,arr => i/arr.length) );
geometry.setAttribute( 'percent', new THREE.BufferAttribute( percents, 1 ) );
const material = new THREE.ShaderMaterial({ uniforms, vertexShader: `attribute float percent`, fragmentShader })
new THREE.Points( geometry, material );
```

线路`Line`，见`room/laser`
```ts
const geometry = new THREE.BufferGeometry().setFromPoints( Vector3[] ); // 可为连续线
new THREE.Line(geometry, new THREE.LineBasicMaterial({ color:'#FF0000' }));
```

const geometry = new THREE.BufferGeometry().setFromPoints( points );

ExtrudeGeometry CatmullRomCurve3

## 画地图、Line2一般曲线

```ts
json.features.forEach((element) => {//循环json.features
    let shapeArray: THREE.Shape[] = []//多面数组
    const color = GetRandomColor()//随机生成16进制颜色
    switch(element.geometry.type){
        case 'LineString': 
        case 'Point': 
        case 'MultiPolygon': 
    }
})
const LineString = ()=>{
    const pts = element.geometry.coordinates.map(pt => new THREE.Vector2(pt[0], pt[1]).multiplyScalar(scale))
    // 方案一 cga.extrudeToGeometryBuffer([cga.v3(-T/2, 0, 0), cga.v3(+T/2, 0, 0)], pts, opt);
    // 方案二（需着色器）：new THREE.Line( BufferGeometry.setFromPoints(pts), material )
    // 方案三：new THREE.CatmullRomCurve3(pts)
    //b23.tv/mfrQbCy
    const spline = new THREE.CatmullRomCurve3(pts.map(pt => new THREE.Vector3(pt.x, pt.y, 0)))
    const positions = Array.from({length: pts.length}).map((_,i) => spline.getPoint(i).toArray())
    const geometry = new LineGeometry()
    geometry.setPositions(positions.flat())
    const color = new THREE.Color().setHSL(Math.random()*2*Math.PI, 1.0, 0.5).getHex()
    const material = new LineMaterial({
        color,
        // vertexColors:true 如果要渐变色 geometry.setColors()
        worldUnits: false, // 使用像素，但需设置resolution。否则使用Three单位，但宽度不定
        linewidth: 2,
        // dashed... // 间断线
    })
    material.resolution.set(window.innerWidth, window.innerHeight) // worldUnits
    const mesh = new Line2(geometry, material)
    mesh.computeLineDistances() // 计算线条长度
    group.add(mesh)
}
const Point = ()=>{
    const pt = new THREE.Vector2(...element.geometry.coordinates).multiplyScalar(scale)
    const geometry = new THREE.CircleGeometry(markRadius, 6)
    const material = new THREE.MeshBasicMaterial({ color: GetRandomColor() })
    const circle = new THREE.Mesh(geometry, material)
    circle.position.set(pt.x, pt.y, 0)
    group.add(circle)
}
const MultiPolygon = ()=>{
    element.geometry.coordinates.forEach(coordinate => {//循环每一个面
        coordinate.forEach(face => { // 循环面的每一个顶点
            // 面的顶点数据 转化为Vector2构成的顶点数组
            const points = face.map(pt => new THREE.Vector2(pt[0], pt[1]).multiplyScalar(scale));
            let shape = new THREE.Shape(points);
            shapeArray.push(shape)
        });
    });
    const is_water = 'water' === element.properties?.natural;
    const geometry = new THREE.ExtrudeGeometry(shapeArray, {
        depth: is_water ? 0 : maxHeight * Math.random(),//拉伸长度
        bevelEnabled: false//无倒角
    });
    // geometry.center();//几何体居中
    const material = new THREE.MeshPhongMaterial({
        color: color,
        side: THREE.DoubleSide //两面可见
    }); //材质对象
    const polygon = new THREE.Mesh(geometry, material)
    polygon.name = element.properties?.name
    group.add(polygon)
}
```

# bug

https://github.com/element-plus/element-plus/issues/1886

`Tab3YunPage.vue`中的fullscreen需在退出播放时触发为false

`yun/index.vue`中的`<template>`不行但`<div>`可用

`yun/index.vue`中的`(r.prefixes || []).forEach`尽管提示为`string[]`但有时确实为`undefined`，却又无法用if判断出来

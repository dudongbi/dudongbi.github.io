---
title: 1vue-opx
date: 2023-02-09 14:40:08
tags: [vue,ts]
---

# OPX依赖

```bash
yarn create vite <my-project> --template vue-ts
cd <my-project>
yarn
yarn upgrade-interactive --latest

yarn add -D sass
yarn add -D @types/node # vite.config.ts 找不到 path
yarn add -D @types/lodash-es # element 找不到类型
yarn add -D type-fest # element 找不到类型
```

```bash
# vue
yarn add pinia
yarn add axios vue-axios
yarn add vue-router@^4
yarn add vue-i18n@next
yarn add vue3-count-to
yarn add vuedraggable@next
yarn add normalize.css

# auto element
yarn add element-plus
yarn add -D unplugin-element-plus # 按需样式
// yarn add -D unplugin-vue-components # 按需标签

# DataCenter
yarn add three @tweenjs/tween.js d3 lil-gui xtorcga
yarn add -D @types/three @types/d3

# DocxEditor
yarn add codemirror @codemirror/lang-javascript @codemirror/theme-one-dark
yarn add decimal.js docx html2canvas
yarn add -D @types/katex @types/file-saver
yarn add katex file-saver

# LangClouds
yarn add crypto-js
yarn add -D @types/crypto-js
yarn add highlight.js

# FlowDesign
yarn add bpmn-js preact zeebe-bpmn-moddle camunda-bpmn-js-behaviors bpmn-js-properties-panel
yarn add diagram-js bpmn-moddle camunda-bpmn-moddle
yarn add @types/bpmn-moddle

# FlowImplem
yarn add jspdf
yarn add tui-calendar
yarn add node-imap mailparser
yarn add -D @types/imap @types/mailparser

# mock data
yarn add echarts
yarn add -D @faker-js/faker
yarn add -D mockjs
yarn add -D rollup vite-plugin-mock
```

```bash
yarn dev
yarn build
```

一些废弃的命令
```bash
# vite 自带了
yarn add -D typescript
yarn add -D node-sass
yarn add -D sass-loader

yarn add @tinymce/tinymce-vue
yarn add fuse.js
yarn add xlsx
yarn add jszip
yarn add sortablejs

# preact 冲突
yarn add @fullcalendar/vue3 @fullcalendar/core @fullcalendar/interaction
yarn add @fullcalendar/daygrid @fullcalendar/timegrid @fullcalendar/list
```

# 代理

```ts
// https://juejin.cn/post/7069770431871320078
// ts-node-dev = ts-node + nodemon
/*
INSTALL:
    //help.aliyun.com/document_detail/58011.html#阿里云FC支持到nodejs16
    //docs.serverless-devs.com/fc/yaml/function#runtime#但yaml只到nodejs14
    //help.aliyun.com/document_detail/132044.html#默认custom仅自带nodejs10
    @origin s.yaml "runtime: custom"
    @mod s.yaml "methods: -GET" -> "methods: -OPTIONS -POST"
    npm install -D typescript ts-node-dev @types/node @types/express --registry=https://registry.npm.taobao.org
    npm install -P express --registry=https://registry.npm.taobao.org
DEBUG:
    @set package.json < "dev": "ts-node-dev --respawn --transpile-only ./index.ts"
PRODUCT:
    npx tsc --init
    npx tsc index.ts
    node index.js
FIX:
    npm install node-fetch@2
    npm install -D @types/node-fetch@2
*/
const DEBUG = true
const PORT = 9000 // 阿里云FC统一使用9000端口，见s.yaml的caPort

import fetch_V2, { Response as Response_V2 } from 'node-fetch'

// import express from "express" 是错误的，会导致tsc的js多一个['default']
import express = require("express")
//import qs from 'qs'

const app = express()
app.use(express.json())

const DEBUG_Print = (method: string, requests: Record<string, any>, responses: Record<string, any>) => {
    if (true != DEBUG){
        return
    }
    const r: string[] = [
        '',
        '========================',
        'Forward USER field with method of ' + method,
        ...Object.entries(requests).map(([k,v], i) => {
            return '  ('+i+')  ' + 'Request ' + k + ': ' + JSON.stringify(v, undefined, 4)
        }),
        '========================',
        'Receive DATA field Headers:',
        ...Object.entries(responses).map(([k,v], i) => {
            return '  ('+i+')  ' + 'Response ' + k + ': ' + JSON.stringify(v, undefined, 4)
        }),
        '========================',
        '',
    ]
    console.log(r.join('\n'))
}
const setCORS = (res: any, content_type: any) => {
    res.header('Content-type', content_type)
    res.header('Access-Control-Allow-Origin', '*')
    res.header('Access-Control-Allow-Methods', 'PUT,GET,POST')
    res.header('Access-Control-Allow-Headers', 'Authorization, Content-type')
}

app.options('*', (req, res, next) => {
    DEBUG_Print('OPTION', { headers: req.headers }, {})
    setCORS(res, req.headers['content-type'])
    res.sendStatus(200)
})
app.post('*', async (req, res, next) => {
    const request = {
        url: req.url.slice(1),
        postdata: req.body, // req.read(parseInt(req.headers['content-length'] ?? '0'))
        headers: req.headers
    }
    const response = await fetch_V2(request.url, {
        method: 'POST',
        headers: {'Content-Type': 'application/json'}, // x-www-form-urlencoded https://help.aliyun.com/document_detail/113251.html#POST方法必须设置
        body: JSON.stringify(request.postdata)
    }).catch(err => console.log(err))
    if (response instanceof Response_V2){
        DEBUG_Print('POST', request, { status:response.status.toString(), headers:response.headers })
        setCORS(res, response.headers.get('content-type'))
        // fetch@2 有 const buf = await response.buffer()
        // nodeV18 只有下边的写法
        const buf = Buffer.from(await response.arrayBuffer())
        res.status(response.status).send(buf)
    }
})

// 本地测试，会在s.yaml的methods中被ban掉
app.get('*', (req, res) => res.status(200).send('<h1>Hello World</h1>'))
// 启动
app.listen(PORT, async () => {
    console.log(`App is running at http://localhost:${PORT}`)
})
```
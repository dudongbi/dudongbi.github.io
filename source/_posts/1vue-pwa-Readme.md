---
title: 1vue-pwa
date: 2023-02-09 14:39:08
tags: [vue]
---

# PWA依赖

```bash
npm install -g @ionic/cli@latest
ionic start --help
ionic start pwa tabs --type vue --capacitor --no-deps --no-git
cd pwa
yarn
yarn upgrade-interactive --latest
npx browserslist@latest --update-db

npm install -g @vue/cli
vue add pwa
```

```bash
# bug?
yarn add @babel/core
yarn remove @vue/cli-plugin-e2e-cypress cypress

# tab1
yarn add @ionic/pwa-elements # 摄像头API
yarn add @capacitor/camera

# tab3-ossClient
yarn add ali-oss crypto-js
yarn add -D @types/ali-oss @types/crypto-js

# tab3-hlsPlayer
yarn add video.js
yarn add -D @types/video.js
# yarn add @awesome-cordova-plugins/file-transfer
```

```bash
yarn dev
yarn build --prod
yarn add @capacitor/android
yarn capacitor add android
yarn capacitor copy android
```

環境搭建
---

Node.js (V6.0.0)

1.安裝Cordova和Ionic Beta

```
npm install -g cordova ionic@beta
```

2.Clone工程

```
git clone git@github.com:phodal/growth2.git
```

初始化子模組 content

```
git submodule init
```

```
git submodule update
```


3.執行安裝命令

```
npm install
```

4.執行Web介面

```
ionic serve
```

5.構建、構建手機安裝包

構建:

```
ionic build android
```

直接執行

```
ionic run android
```

Setup for Android
---

Install Cordova,Ionic:

```
npm install -g cordova ionic@beta
```

Plugins:

```
cordova plugin add cordova-plugin-inappbrowser
```

Issue of Setup
---

Cannot find name ‘cordova’:

```
npm install -g typings
typings install dt~cordova --save --global
```

Shell

```shell
typings install dt~cordova/plugins/inappbrowser --save --global
typings install dt~cordova/plugins/splashscreen --save --global
```

Setup Electron Env
---

1. Download Electron from https://npm.taobao.org/mirrors/electron
2. Run ``npm run electron``

### Convert md to HTML

```shell
find ./ -iname "*.md" -type f -exec sh -c 'pandoc "${0}" -o "html/${0%.md}.html"' {} \;
```

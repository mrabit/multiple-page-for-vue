# vue-cli 的多页面应用构建

> Vue构建的大多是SPA单页面应用,但有时候在实际项目中单页面应用并不一定符合业务需求

代码具体实现在:  [vue-cli的多页面应用构建](https://blog.mrabit.com/details/48 "vue-cli的多页面应用构建")

### 运行使用

``` shell
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev
```

### 文件结构
```shell
.
├── README.md
├── build
│   ├── build.js
│   ├── check-versions.js
│   ├── logo.png
│   ├── utils.js
│   ├── vue-loader.conf.js
│   ├── webpack.base.conf.js
│   ├── webpack.dev.conf.js
│   └── webpack.prod.conf.js
├── config
│   ├── dev.env.js
│   ├── index.js
│   └── prod.env.js
├── package.json
├── src
│   ├── assets
│   │   └── logo.png
│   ├── components
│   │   ├── Hello.vue
│   │   └── cell.vue
│   └── module
│       ├── cell
│       │   ├── cell.html
│       │   ├── cell.js
│       │   └── cell.vue
│       └── index
│           ├── index.html
│           ├── index.js
│           ├── index.vue
│           └── router
│               └── index.js
└── static
```
`src` 为默认工程文件,其中的 `assets` , `components` , `module` 分别是静态资源文件、组件文件、页面文件。
页面文件中按照项目的模块分的文件夹,每个文件夹下分别有三个内容：vue文件，js文件和html文件。这三个文件的作用就相当于做spa单页面应用时，根目录的 `index.html` 页面模板，src文件下的 `main.js` 和 `app.vue` 的功能。

参考地址:
- [用vue构建多页面应用](https://segmentfault.com/a/1190000011265006 "用vue构建多页面应用")

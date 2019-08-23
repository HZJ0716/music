# music

vue2 + vue-router2 +vuex + jsonp + es6 +webpack <br>
数据来源:QQ音乐接口使用

# 技术栈

- Vue：用于构建用户界面的 MVVM框架。它的核心是响应的数据绑定和组系统件
- vue-router：路由系统，使用Lazy Loading Routes 异步加载优化性能
- vuex：Vue 集中状态管理，组件共享状态信息
- vue-lazyload：图片懒加载库，优化页面加载速度
- better-scroll：滑动处理
- stylus：css 预编译处理器
- ES6 

【后端】

- Node.js
- jsonp：伪造数据头获取音乐数据
- axios：异步请求数据

【自动化构建及其他工具】

- webpack：项目的编译打包
- vue-cli：Vue 脚手架
- eslint

## 推荐

`better-scroll` 实现滚动效果，使用 `jsonp` 获取QQ音乐数据

`axios` +` Node.js` 伪造头部获取数据并跨域

`vue-lazyload` 图片懒加载提高用户体验

## 歌单详情

`vuex` 管理歌手状态, 动画拉伸放大等

## 播放器

 `vuex` 管理播放器状态，使用html5 `audio` 控制播放，暂停等

 调整歌单列表数组顺序完成顺序播放、单曲循环、随机播放

歌词的爬取利用 `axios` 代理后端请求，伪造 `headers` 来实现，先将歌词 `jsonp` 格式转换为 `json` 格式，再使用第三方库 `js-base64` 进行 `Base64` 解码操作，最后再使用第三方库 `lyric-parser` 对歌词进行格式化

## 搜索页

`localstorage` 对搜索历史进行缓存

## 个人中心

将 `localstorage` 中存储的相关信息显示

# 安装与运行
```
npm install //安装依赖

npm run dev //服务端运行 访问 http://localhost:8080

npm run build  //项目打包 
```

For a detailed explanation on how things work, check out the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).

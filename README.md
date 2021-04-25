> ### 基于koa2实现一个模拟接口数据的本地服务器

> ### 1.创建koa2项目

1. 安装 koa-generator脚手架

`npm install koa-generator -g`

2. 一键生成koa2项目

`koa2 xxx` 

3. 安装依赖

`npm install`

生成的koa2项目目录如下

```
xxx/
|
+——bin/
|   |
|   +—— www     程序入口
|
+——public/      静态资源
|   |
|   +—— image/   
|   +—— javascripts/
|   +—— stylesheets/
|
+——routes/      路由配置
|   |
|   +—— index.js
|   +—— users.js
|
+——views/       页面模板引擎
|   |
|   +—— error.pug
|   +—— index.pug
|   +—— 
|
+——app.js       使用koa的js
|
+——package.json
```
**bin/www** 是入口文件，打开端口监听(默认3000)，启动koa服务

**app.js** 是使用koa的js，里面已经配置好了，解析http请求、使用静态资源、log埋点、使用路由等中间件。

## Project setup
```
yarn install

yarn start
```

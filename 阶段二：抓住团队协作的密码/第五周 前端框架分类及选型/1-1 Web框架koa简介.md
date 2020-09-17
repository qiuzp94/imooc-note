## 章导学
* **Koa简介,工作原理**
* 安装&配置Koa,常用中间件介绍
* Koa开发调试

## 思维导图
### Koa介绍
#### Koa简介
* 功能
* 核心概念
    * 应用
    * 请求
    * 上下文
    * 响应
* 特点
    * 轻量/简洁
    * async/await支持

#### Koa使用
* 安装
    * npm install -S koa
    * 版本依赖
        * nodejs>v7.6.0
* Koa中间件
    * Koa工作原理
* 常用插件 **(重点)**
    * 路由 koa-router
    * 跨域处理 @koa/cors
    * 压缩 koa-compress
    * 静态资源 koa-static
    * 协议处理
        * koa-json
        * koa-body
    * 安全
        * 鉴权方式
            * koa-session
            * koa-jwt
        * 通信头 koa-helmet
    * 日志 koa-logger
* 常用API
    * app.use
    * app.listen
    * app.on

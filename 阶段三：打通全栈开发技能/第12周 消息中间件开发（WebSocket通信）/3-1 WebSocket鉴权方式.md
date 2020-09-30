## Websocket鉴权
* 协议本身在握手阶段不提供鉴权方案
* 浏览器侧:url传参，message主动消息，session/cookie
* **Nodejs侧:直接使用ws传Headers**
## 一、工作中的痛点问题的解决方案
* 对组织人员培训，**转变思维**向自动化/规范化转型
* 配合效率工具（自动化）对**流程**进行**简化**标准化
* **全员参与**并实践

## 二、DevOps内容介绍（重点）
### 敏捷流程
  plan code build test release deploy operate monitor  -> 回到最开始的 plan 

版本管理、自动化、文档管理、缺陷控制都是围绕着上面的循环展开的

  Dev Ops
 
### 一般项目DevOps内容介绍
#### Project
* ↓
* 版本控制 主干与分支   git、svn    github、gitee  【git flow】
* ↓
* 自动化平台打包 / PANCHER（管理集群化的结点，稳定性的服务，部署到各种云平台） 【自动化流程】
* ↓
* Dev Prod Test/UAT 【自动化流程】



#### 开发人员 
* ↓
* IDE编程   【本地开发】
* ↓
* Docker容器    【本地开发】
* ↓
* JIRA 缺陷控制 -> OK则 版本控制 主干与分支 / BUG则 退回Docker容器 【缺陷管理】
* ↓
* 文档管理 API  【缺陷管理】
* ↓
* 测试-> JIRA 缺陷控制  【缺陷管理】


#### 测试人员
* ↓
* ARMA、JASMINE、JEST、MOCHA 【本地测试】



## 题目
如何创建一个在3306端口的容器名称为mysql的Mysql容器，创建后在后台持续运行？

```
docker run -itd --name mysql -p 3306:3306 -e=MYSQL_ROOT_PASSWORD=123456 mysql
```

* docker run 命令来创建
* itd交互式终端后台运行
* name指定容器名称
* p指定映射端口
* 最后Mysql比较特殊，需要指定MYSQL_ROOT_PASSWORD变量 + mysql镜像名称

## 题目二
文件、资源、网络隔离、写是复制、独立的资源划分是Docker容器技术的特点



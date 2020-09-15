nvm: Node Version Manager

因为vue-cli需要node 8.9版本以上，所以我们可以用nvm来管理node

## 一、nvm
### 1.1 下载安装
#### Macos与Linux


https://github.com/nvm-sh/nvm

```
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.3/install.sh | bash
```

然后nvm的环境变量添加到系统上

Running either of the above commands downloads a script and runs it. The script clones the nvm repository to ~/.nvm, and attempts to add the source lines from the snippet below to the correct profile file (~/.bash_profile, ~/.zshrc, ~/.profile, or ~/.bashrc).


```
export NVM_DIR="$([ -z "${XDG_CONFIG_HOME-}" ] && printf %s "${HOME}/.nvm" || printf %s "${XDG_CONFIG_HOME}/nvm")"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh" # This loads nvm
```



#### Window

https://github.com/coreybutler/nvm-windows

release -> Assets -> nvm.setup.zip

### 1.2 nvm 相关命令
* `nvm --version` 查看nvm版本
* `nvm -help` 查看帮助
* `nvm install 8.0.0` 安装node 8.0 版本
* `nvm use 8.0` 切换使用到node 8.0 
* `nvm list` 查看本地node的版本


其他命令建议查看`nvm -help` 

## 二、yarn--前端包管理工具(Macos)

[官网](https://classic.yarnpkg.com/zh-Hans/docs/install/#mac-stable)

### 安装下载
方法一

`brew install yarn`

方法二

```
curl -o- -L https://yarnpkg.com/install.sh | bash
```

### 简单使用
* `yarn -v` 查看版本
* `yarn config get registry` 查看本地yarn使用的源
* `yarn config set registry 'https://registry.npm.taobao.org/'` 将查看本地yarn源切换到淘宝源

* `yarn global add @vue/cli` 全局安装vue/cli工具
* `yarn install xxx` 安装xxx的依赖包
* `yarn add xxx` 添加xxx的依赖包

其他命令，可以通过[官方文档查阅](https://classic.yarnpkg.com/zh-Hans/docs)，可以通过`yarn --help`了解其他指令

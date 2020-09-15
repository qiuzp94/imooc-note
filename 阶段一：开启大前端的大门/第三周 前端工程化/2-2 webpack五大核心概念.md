## Webpack&gulp

https://www.webpackjs.com/ 

### Webpack 核心概念
#### 入口

``` javascript
 moddule.exports={
     entry:'./path/to/my/entry/file.js'
 }

```

#### 输出

``` javascript
    const path = require('path');

    module.exports = {
        entry: './path/to/my/entry/file.js',
        output:{
            paht:path,resolve(_dirname,'dist'),
            filename:'my-first-webpack.bundle.js'
        }
    };
```

#### Loader(载荷)

``` javascript
    const path = require('path');

    module.exports = {
        output:{
            filename:'my-first-webpack.bundle.js'
        },
        module:{
            rules:[
                {
                    test:/\.txt$/,use:'raw-loader'
                }
            ]
        }
    };


```

#### 插件

``` javascript
    
    const HtmlWebpackPlugin = requeire('html-webpack-plugin');//通过npm安装
    const webpack = require('webpack');//用于访问内置插件

    module.exports = {
        module:{
            rules:[
                {
                    test:/\.txt$/,use:'raw-loader'
                }
            ]
        },
        plugins:[
            new HtmlWebpackPlugin({template:'./src/index.html'})
        ]
    };


```

#### 模式/兼容性

webpack 支持所有符合ES5标准的浏览器（不支持IE8及以下版本）。
webpack的import()和require.ensure()需要Promise。
如果想要支持旧版本浏览器,在使用这些表达式之前，还需要**提前加载polyfill**

`npm install --save babel-polyfill`

然后，使用import 将其引入到我们的主bundke文件:

src/index.js

``` javascript
import 'babel-polyfill';

function component(){
    var element = document.createElement('div');
    
    element.innerHTML = join(['Hello','webpack'],'');

    return element;
}

document.body.appendChild(component());
```

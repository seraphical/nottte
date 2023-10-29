- 是一个环境
- 私人: 一个'软件', 你电脑执行某功能的能力
    - 栗子: 你的电脑的office环境
    - 栗子: 电脑的node环境
- 是一个把js解析引擎独立出来, 安装在你的电脑上
    - 让你的电脑有了独立运行js 代码的能力
- 官方 : 一个基于Chrome V8 解析引擎的运行时环境

# 前端js
- DOM
    - 因为js 被引入了html页面
    - 所有的Dom 结构都依赖于html结构运行
    - 我们的 js 是在一个页面里面运行的, 在文档流内
- BOM
    - 因为最终这个文件被引入了浏览器执行
    - 操作浏览器的部分内容
- ECMAScript
    - js的语法

# 后端JS (node)
- ECMAScript
- I/O 输入/输出
- system
- server

# js
- 代码不区分前后端
- 区分你的执行方式
- 将来你需要把这一段js 代码, 放在html文件内引入, 在浏览器打开
    - 那么你的代码就需要书写关于Dom/Bom的操作
    - 不能操作文件, 操作系统之类的内容
- 将来你需要把一段js代码, 放在node环境中运行
    - 那么你的代码就需要书写关于 文件, 操作系统种类的内容
    - 不能操作 Dom/Bom相关的内容


# node 环境相关
- 输入指令
    - $ node --version
    - 简写: $ node -v
**代码执行**
- 方式1
    - 打开终端
    - 输入指令
        - $ node
    - 会进入js代码编辑环境
        - 相当于浏览器的控制台
        - 可以直接书写js代码, 回车后运行

- 方式2 
    - 利用终端来执行一个js文件
    - 需要把代码书写在.js 文件内
    - 打开终端
    - 切换终端目录(重点)至当前文件所在目录
    - 输入指令
        - $node 文件名
    - 会在终端内以 node 环境来运行当前的js文件


# 模块化语法
## exports
```js
//a.js
const a = 1;
const b = 2;

exports.a = a;
exports.b = b;
```
使用 `exports.变量 = 变量`在另一个文件内导入使用`require`解构方式

```js
const { b ,a} = require('./a');
console.log(b,a); // 2,1
```

## module.exports
```js
//a.js
const a = 1;
const b = 2;
module.exports = {a,b}
```
这种方式可以一次性导出多个, 导入的时候则不需要结构就可以拿到导出的东西
```js

const Module= require('./a');
console.log(Module); // {a:1,b:2}
```


# 模块
## fs
- 叫做file system 模块
- 专门用来操作文件的模块
- 直接导入使用即可

1. fs.readFile
    - 语法: `fs.readFile (文件地址, [格式], 回调函数)`
    - 格式: 默认读取的buffer 格式字符串, 我们可以选填'utf-8'
    - 作用: 异步读取文件信息

2. fs.readFileSync
    - 语法: `fs.readFileSync (文件地址, [格式])`
    - 作用: 同步读取文件信息
    - 返回值: 该文件内的信息

3. fs.writeFile( )
    - 语法: fs.writeFile (文件地址, 写入内容, 回调函数)
    - 作用: 异步写入文件内容
    - 注意: 完全覆盖式的写入内容
    - 注意: 当你写入的时候, 如果没有这个文件, 会自动创建这个文件写入


## path
- 专门用来操作路径相关信息的模块
- ==注意: 使用join或者resolve拼接起来的路径不能和字符串相加==

1. join( )
    - 语法: path.join(路径信息1,路径信息2 ..........)
    - 返回值: 把多个路径信息组装在一起, 返回一个相对路径

2. resolve( )
    - 语法: path.resolve(路径信息1, 路径信息2.......)
    - 返回值: 把多个路径信息组装在一起, 返回一个绝对路径


3. parse( )
    - 语法: path.parse( 路径信息)
    - 返回值: 是一个对象数据类型, 保存的就是该路径内的所有信息



## url
- 存储的都是关于url地址的信息
- url.parse( )
    - 语法: `url.parse( url地址,[ 是否深度解析])`
    - 是否深度解析: 是否解析查询字符串内容, 默认是false, 选填true
    - 返回值: 是一个对象数据类型, 存储的就是该url 内解析出来的信息
    - 注意:==参数中的url地址必须带有问号(?)才能够解析出search和query==

注意与 path.parse 的区别
- ==path.parse 主要用来解析出标识符的后缀, 文件名等==
- ==url.parse 主要用来解析出标识符中的查询字符串和获得查询字符串深解析之后的对象==


## http模块
- 专门用来开启一个http服务的模块
    - 利用这个模块可以把js文件在cmd运行的状态变成一个服务器

1. 地址标识符
    - 前后端约定好的一个标志
    - 栗子
        - 服务器: 
            - 我有一个index .html文件
            - 做了一个服务器处理
            - 当前端需要访问这个index.html文件的时候, 只要告诉我请求/aaa
        - 客户端
            - 当你需要访问这个index.html文件的时候
            - 你只需要发送一个请求, 请求地址书写/aaa即可

2. 服务器
    - 一个提供服务的机器
    - 服务
        - 根据前端的请求给出一个 文件(html,  css, js, jpg, wmv..)
        - 根据前端的请求给出一个数据
    - 什么叫做前端的请求(向服务器索要内容)
        - 注意: 请求内的地址是一个标识符, 不是真正的文件地址
        - ==地址栏书写地址==
            - `http://localhost:8888/a/index.html`
            - 向服务器发送了一个get请求, 请求地址是/a/index.html
        - ==link标签的href属性==
            - `<link href = "http://localhost:8888/a/index.css">`
            - 向服务器发送了一个get请求, 请求地址是/a/index.css
        - ==script 标签的 src 属性==
            - `<script src="http://localhost:8888/a/index.js"></script>`
            - 向服务器发送了一个 get 请求, 请求地址是 /a/index.js
        - ==ajax请求==
            - 根据你配置的请求地址和请求方式
            - 决定向服务器发送get或者post请求, 地址是你填的url


# 简易服务器

## 最简服务器
```js
const http = require('http')

const app = http.createServer((req,res)=>{
	res.end()
})

app.listen(4000,()=>{

})
```
**创建服务createServer**
- 语法: `http.createServer(function( ){     })`
- 意义: 创建了一个服务, 只要将来有==任何==请求来到这个服务的时候都会触发函数
- 返回值: 一个服务
- request(req): 每一次请求相关的信息
- response(res): 每一次请求所需要的响应信息, 我们向res内添加的内容将来都会被node自动组装成响应报文返回给前端
- request内有一个叫做url的信息, 表示本次请求地址(==标识符==)
- request内有一个叫做headers的信息, 表示本次请求的请求头
- 读取文件成功后
- 把data信息返回给客户端即可
- 语法: res.end( 返回给客户端的信息)
- ==注意: 只能返回字符串类型==

**listen**
- 服务器: 找到某一台电脑, 运行一个端口号
- 语法: 服务.listen( 端口号, 回调函数)
注意: 当使用cmd窗口去运行这个app.js文件的时候, 当前cmd窗口就是一个服务器
## 一个读取文件的接口
```js
const http = require('http');
const fs = require('fs');
const path = require('path');
const url = require('url');
// http://localhost:8080/readFile?name=jack&age=18

var defaultCorsHeaders = {
  'access-control-allow-origin': '*',
  'access-control-allow-methods': 'GET, POST, PUT, DELETE, OPTIONS',
  'access-control-allow-headers': 'content-type, accept, authorization',
};

const app = http.createServer((req, res) => {
  res.writeHead(200, defaultCorsHeaders);

  const { pathname, query } = url.parse(req.url, 'true');
  if (pathname == '/readFile') {
    console.log(query);
    const data = fs.readFileSync(
      path.resolve(__dirname, './index.html'),
      'utf-8',
    );
    res.end(JSON.stringify(query));
  }
});

app.listen(8080, () => {
  console.log('服务创建成功');
});
```
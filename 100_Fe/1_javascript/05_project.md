![[link/Pasted image 20231022140935.png]]


# url
`http://127.0.0.1:5500/chatterbox.html?username=%E5%95%8A%E5%95%8A%E5%95%8A`
- https/http
   - 协议 protocol
   - 规定通信的流程,比如使用什么通信,通信要携带什么内容,三次握手,4 次挥手,状态码标识什么意思
-  host
   - ip 或者域名
      - 域名和 ip 的关系是什么:ip 是一串数字,域名是方便记忆的,这两个其实一样
      - 怎么通过域名找到 ip=> dns 解析
   - `127.0.0.1 == localhost`
- port
   - 5500
- /chatterbox.html?username=%E5%95%8A%E5%95%8A%E5%95%8A
   - 路径

## ip 和 api(接口)
api 包括(接口)
- url
- method:get / post
- body=>data
- content-type 属于 header

# websocket
相当于一直建立连接,所以可以进行实时通信


# http 请求
相当于打电话的过程
- 请求头 header
- 请求体 body
- 请求方法

**header中常用的配置**
- content-type 表示我要给服务端上送的内容格式
   - json 字符串: application/json   json
   - 二进制流字符串: multipart/form-data    文件使用的格式 流格式
   - 查询字符串: application/x-www-form-urlencoded   form 表格常用的格式 querystring
- Authorization 这玩意是校验用的,验证身份用的,是后端给你的
   - token
- 可以设置 cookie

**cookie**
 cookie 属于 bom 的内容, 发送请求的时候会自动带上 cookie
   - 保存登录信息的, 后端把用户数据返回, 可以存在 cookie 中让他自动带给后端
**body** 请求体
提交信息方式的区别,get 使用地址栏传参,post 使用请求体传参
get 方式发送数据, 在地址栏携带数据, ?后面的 queryString 就是要上送的数据
- querystring
   - ?address=china&name=xiaoming&age=12
post 方式发送数据, 在请求体中携带数据
- jqery 中放在 data,不能直接发送一个对象或者数组, 通信格式一般是 json



# restful
用 get 方式上送一个 name
- http://xxxx:4000/?name=xiaoming
使用偷懒方式
- http://xxxx:4000/xiaoming



# project

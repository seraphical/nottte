记得做昨天的作业

# 代码讲解
## 第一次出现偶数个的项
**你自己的代码**
```js
// 找到数组中最先出现偶数次的一项
var evenOccurrence = function (arr) {
  // Your code here.
  //[[1],[7],[2],[4,4],[5],[6,6],[8],[9];
  let result = [];
  // arr[0] - > find if not same -> push to single and single send result;
  // -> if same -> push other to single- > finally push itself and send result;
  // and then iterate every single;
  for (var i = 0; i < arr.length; i++) {
    let everysingle = [];
    for (var a = i + 1; a < arr.length; a++) {
      if (arr[i] === arr[a]) {
        //[1,  , , 7, 2, 4, 5, 6, 8, 9, 6, 4]
        everysingle.push(arr[a]); // [1,1,1]
        delete arr[a]; //?
      }
    }
    everysingle.push(arr[i]);
    result.push(everysingle); //[[1,1,1],]
    a++;
  }

  [[1,1,1],[7],[2],[4,4],[8,8]...]
  var finalresult ;
  // console.log(finalresult);
  for (var i = 0; i < result.length; i++) {
    // console.log(result[i]);  []
    if (result[i].length&&result[i].length % 2 === 0) {
      if(finalresult) return
      finalresult =  result[i][0]
    }
  }

};
var onlyEven = evenOccurrence([1, 1, 1, 7, 2, 4, 5, 6, 8, 9, 6, 4]);
console.log(onlyEven); //  4
```
实现思路基本正确, 一些代码细节和特性需要注意
`delete arr[index]` 基本不使用, 并且这样执行会造成数组塌陷
`if(finalresult) return` 这是流程控制的常用手段 和 flag 类似


**我的代码**
```js
// 找到数组中最先出现偶数次的一项

const even0ccurrence = (arr) => {
  let returnVal = null,
    count = 0,
    flag = false;
  //首先对这个数组去重,就是每个项只出现一次
  let dedupulicateArr = [...new Set(arr)]; //[ 1, 7, 2, 4,5, 6, 8, 9 ] 数组去重

  dedupulicateArr.forEach((item) => {
    arr.forEach((v) => {
      if (item == v && !flag) count++;
    });

    if (count % 2 == 0 && count) {
      returnVal = item;
      count = 0;
      flag = true;
    } else {
      count = 0;
    }
  });

  return returnVal;
};

var onlyEven = even0ccurrence([1, 1, 1, 7, 2, 2, 2, 4, 5, 6, 8, 9, 6, 4]);

console.log(onlyEven);
```
`let dedupulicateArr = [...new Set(arr)]; ` 数组去重的方式之一

本题涉及知识点: 流程控制和数组去重


## hashTable
```js
Hashtable: var HashTable = function () {
  this._limit = 8;
  this._storage = LimitedArray(this._limit); //~    [1,2,3,4,5,6,7,8]
  //console.log('this._storage', this._storage);
};

HashTable.prototype.insert = function (k, v) {
  //[key1:valueaaaa]
  var index = getIndexBelowMaxForKey(k, this._limit);
  var buckets = this._storage.get(index) || [];

  // check if there's an element with the same key in the bucket (collision)
  for (var i = 0; i < buckets.length; i++) {
    var array = buckets[i];

    if (array[0] === k) {
      array[1] = v;
      // this._storage.set(index, v);
      return;
    }
  }
  // then we have to set the key
  buckets.push([k, v]);
  this._storage.set(index, buckets);
};

HashTable.prototype.retrieve = function (k, v) {
  var index = getIndexBelowMaxForKey(k, this._limit);
  var buckets = this._storage.get(index, v) || [];

  for (var i = 0; i < buckets.length; i++) {
    var array = buckets[i];

    if (array[0] === k) {
      // this._storage.set(index, v);
      return array[1];
    }
  }
};

HashTable.prototype.remove = function (k) {
  var index = getIndexBelowMaxForKey(k, this._limit);
  var bucket = this._storage.get(index);

  if (bucket) {
    for (var i = 0; i < bucket.length; i++) {
      var currentBucket = bucket[i];
      if (currentBucket[0] === k) {
        bucket.splice(i, 1);
        return;
      }
    }
  }
};
```
哈希表的工作原理是使用一个**哈希函数**将键转换为一个索引，然后将值存储在这个索引对应的位置。当你需要查找一个值时，哈希表会使用同样的哈希函数将键转换为索引，然后直接访问这个索引对应的位置来获取值。这使得哈希表的查找速度非常快，理想情况下，查找的时间复杂度可以达到 O(1)。

但是，哈希表也有一些问题。例如，不同的键可能会被哈希函数转换为同一个索引，这被称为哈希冲突。解决哈希冲突的方法有很多，例如**链地址法**（将冲突的值存储在一个链表中）或**开放地址法**（寻找下一个空的位置）。

上面的代码使用的就是链地址法来解决哈希冲突
![[link/Pasted image 20231021012310.png]]
```js
HashTable.prototype.insert = function (k, v) {
  //[key1:valueaaaa]
  var index = getIndexBelowMaxForKey(k, this._limit);
  var buckets = this._storage.get(index) || [];

  // check if there's an element with the same key in the bucket (collision)
  for (var i = 0; i < buckets.length; i++) {
    var array = buckets[i];

    if (array[0] === k) {
      array[1] = v;
      // this._storage.set(index, v);
      return;
    }
  }
  // then we have to set the key
  buckets.push([k, v]);
  this._storage.set(index, buckets);
};
```
要插入一个值, 先根据 key 生成 index,然后根据index 找到 hashTable 中处在 index 位置的 buckets, 遍历这个 buckets
- 如果要插入的值的 key 和当前正在遍历的 buckets 的这一项的 key 相同, 则会对其进行覆盖
- 如果遍历整个 buckets 都没有发现与要插入值的 key 相同的 key 就把这个值 push 进 buckets 中


# 提前了解
## 位运算符 >> <<
左移（<<）：将操作数的所有位向左移动指定的位数，右侧用0填充。
```js
   a = 5  // 二进制表示为 0101
   result = a << 2  // 结果为 10100，即 20
```
右移（>>）：将操作数的所有位向右移动指定的位数，左侧用符号位（对于有符号数）或0填充
```js
   a = 5  // 二进制表示为 0101
   result = a >> 1  //结果为 0010，即 2
```


## 事件轮询 event-loop
在事件轮询模型中，程序会不断地检查是否有待处理的事件，如果有，则立即处理它们，否则继续等待。这种方式避免了阻塞线程，提高了程序的响应性能。

事件轮询的基本原理是将事件添加到事件队列中，然后按照顺序依次处理队列中的事件。当事件被触发时，相应的回调函数会被调用。这种模型适用于处理各种类型的事件，例如用户输入、网络请求、定时器等。


# ajax
## 前后端交互
 一. 前后端交互
- 前端和后端进行数据通讯 (在网络中只能传递字符串)
- 目前需要学习
    - 如何向后端发送一个请求(request)
    - 如何接受后端给回的一个响应(response)
- 目前常用的请求协议
    - http/https
    - socket

### http传输协议
- 协议: 约定好的内容
- 约定
    - http请求, 只能由前端主动发起
    - 传递的内容只能是字符串
    - 前端给到后端的请求必须要以请求报文的形式
    - 后端给到前端的响应必须要以响应报文的形式
    - 前后端交互必须遵守一次请求一次响应的规则
    - 需要遵守一个固定的步骤


### http传输协议的步骤
- 步骤1: 建立前后端的连接
    - 基于TCP/IP协议的三次握手



- 步骤2: 前端以请求报文的形式发送本次请求(浏览器会自己组装)
    - 请求报文行
        - 传输协议版本: HTTP/1.1
        - 请求方式: '前后端说话的方式'
        - 请求地址: 你向哪一个服务器发送
    - 请求报文头(包含本次请求的说明信息, 给服务端看的)
        - origin : 从哪来的
        - userAgent: 浏览器信息
        - cookie: 只要cookie空间内有内容, 会自动携带
        - cotent-type: 传递给后端的数据类型是什么
        - accept: 期望后端返回的数据类型(图片格式/ html格式)
    - 请求报文空行
        - 分隔请求报文头和请求报文体
    - 请求报文体
        - 前端需要传递给后端的信息
        - 前端给到后端的数据



- 步骤3: 前端接受后端返回的响应报文(浏览器会自动解析报文)
    - 响应报文行
        - 传输协议版本: HTTP/1.1
        - 本次响应状态码: 以一个数字表示本次请求状态
        - 对本次响应的简单描述
    - 响应报文头(对本次响应的简单描述信息)
        - server: 服务器信息
        - Date : 服务器事件(世界标准时间)
        - content-length: 响应体长度
        - content-type: 响应体数据格式
    - 响应报文体
        - 后端返回给前端的具体信息
- 步骤4: 断开前后端的连接
    - 基于TCP/IP协议的四次挥手
    - 目的: 为了保证前后端是正常断开连接




## ajax

### 请求方式
- 是前后端约定好的一个通讯"规则"
- 就是一个语义化的区别
- 常见的请求方式
    - GET : 偏向获取的语义
    - POST:偏向提交的语义
    - PUT: 偏向提交的语义, 偏向提交存储
    - DELETE: 偏向删除的语义
    - PATCH: 偏向提交的语义, 偏向提交修改
    - HEAD: 偏向获取的语义, 获取响应头信息
    - OPTIONS: 偏向获取的语义, 获取服务器信息(需要服务器统一)
    - CONNECT: 保留方式, 管道连接改为代理连接使用

#### GET 和 POST 的区别
1.  语义化不同
2.  携带参数的位置
    - GET 请求: 直接以查询字符串的形式拼接在地址的后面
    - POST 请求: 把信息书写在请求体内
3.  携带参数的大小不一样
    - GET 请求: 一般不超过 2kb
    - POST 请求:原则上不限制大小, 但是可以被服务器限制
4.  携带参数的格式不一样
    - GET 请求: 只能携带查询字符串格式
    - POST 请求: 可以携带多种格式数据, 但是需要在请求头内做出说明
        - 查询字符串: application/x-www-form-urlencoded
        - json 字符串: application/json
        - 二进制流字符串: multipart/form-data
5.  安全性(相对)
    - GET 请求: 明文发送, 相对不安全
    - POST 请求: 暗文发送, 相对安全

- 栗子:
    - 登录
        - 前端: 把用户名和密码发送过去
        - 后端: 返回 对 或者 不对
    - 注册
        - 前端: 把用户名和密码发送过去
        - 后端: 返回 成功 或者 失败
    - 新闻列表
        - 前端: 需要 什么新闻, 多少条, 第几页
        - 后端: 返回一个新闻列表

### 响应状态码
- 在报文内对于本次响应的状态的描述
- 响应状态码分类
    - 100~199    表示连接继续
    - 200~299    表示各种成功
    - 300~399    表示重定向
    - 400~499    表示客户端错误
    - 500~599     表示服务端错误

#### 重定向
- 在前后端交互的过程中
- 前端  ---------> 后端 A
- 当后端 A 接收到前端的请求后, 告诉前端, 你去请求 后端 B
    - 此时前端会自动把本次请求-------------> 后端 B
    - 最终由后端 B 给前端返回信息
- 常见
    - 304  缓存
    - 301 永久重定向
    - 302  临时重定向

- 判断请求完成的时候
    - 可以通过完成事件 + 响应状态码来决定

### 发送请求
#### 了解如何访问服务器
- 前提: 保证服务器的开启
- 请求
    - 找到服务器: 找到端口号, 找到服务器提供的地址
    - 找到服务器: 通过域名(IP)
    - 找到端口号: 通过端口号, 找到指定哪一台电脑上的软件, 目的找到开放文件夹
    - 找到提供的地址: 不是文件夹内的路径地址, 只是一个请求标识符而已(暗号)
        - 你想要[新闻列表] , 你的地址位置书写/aaa
        - 你想要[首页页面] , 你的地址位置书写/bbb
    - 本机 IP
        - 域名: localhost
        - IP: 127.0.0.1

### 如何发送一个请求
- 前端向后端发送请求的技术手段 ajax
    - a: async  异步
    - j: js
    - a: a
    - x: xml   一种严格的 html 格式
- 技术手段的应用
    - 步骤 1: 创建一个 ajax 对象
        - 语法: const xhr = new XMLHttpRequest( )
    - 步骤 2: 配置本次请求的相关信息
        - 语法: xhr.open( 请求方式, 请求地址, 是否异步)
            - 请求方式: 按照接口文档书写
            - 请求地址: 按照接口文档书写
            - 是否异步: 默认是异步, 选填是 false, 表示非异步
    - 步骤 3: 把这个请求发送出去
        - 语法: xhr.send( )
    - 步骤 4 : 接收响应
        - 语法: xhr.onload = function( ){ }
        - 时机: 会在本次请求完成之后触发
        - 在 xhr 内有一个信息, 叫做 responseText 就是本次响应体的全部内容

```js

        //1. 创建ajax对象
        const xhr = new XMLHttpRequest()
        // 2. 配置本次请求相关信息
        xhr.open('GET', 'http://localhost:8888/test/first')

        //3. 把请求发送出去
        xhr.send()
        //4. 接收响应的事件
        // 使用onload是因为接收响应是异步回来的, 需要时间, 而绑定事件是同步的, 若是使用readystatechange就会在响应之前发生绑定,  使得这个事件不会触发, 所以需要onload将事件绑定放在响应完成之后发生
        xhr.onload = function(){
            console.log('请求完成了');
            console.log(xhr.responseText);
        }
```



# 作业
把昨天作业做了


## 数组去重
```js

const  arr  = [
  1, 2, 3, 8, 4, 3, 1,
  3, 4, 5, 6, 3, 2, 1,
  3, 4, 5
]

```
用两种方法把上面的数组去重, 一种是今天学的,另一种随便


## 元素居中
两个正方形,一个大的一个小的, 让小的正方形在大的正方形正中间
![[link/Pasted image 20231021015350.png]]
差不多这个意思

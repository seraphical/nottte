# 作业
## 作业 1
```js

const arr = (array) => {
  // we need sort
  let sortedarray = array.sort((a, b) => a - b); //默认从小到大  默认用字符串比较的
  // we don't need binary search......
  console.log(sortedarray);
  return sortedarray[sortedarray.length - 1]; //找到最大的一个
};

console.log(arr([10, 200, 100, -5, 15, 56, 17]));
```
sort()方法默认从小到大,以字符形式来比较
所以要想以数字形式来比较, 就在里面加上回调 `(a, b) => a - b`

## 作业 2
```html
<body>
    <!-- 实现一个正方形和一个按钮，点击这个按钮的时候能够让正方形切换显示隐藏 -->

    <!-- block, inline-block,inline -->
    <div style="width: 200px;height:200px;background-color: red;"></div>
    <button>button</button>

    <script>

        //display:none
        // opacity:0    
        const oDiv = document.querySelector('div')
        const btn = document.querySelector('button')
        btn.addEventListener('click', () => {
            if (getComputedStyle(oDiv).display === 'none') {
                oDiv.style.display = 'block'
            } else {
                oDiv.style.display = 'none' // style形式只能改样式,不能查样式 , 查样式要通过另一个 api, getComputedStyle()
            }
        })

    </script>
</body>

```
dom 对象(div 和 btn 这种 html 对象通过 querySelector 获取到的就叫做 dom 对象)

通过 `dom 对象.style.样式`这种方式只能够设置, 要通过`getComputedStyle(dom 对象).样式`才能够获取样式

隐藏一个元素的方式
1. display:none
2. opacity:0


**var,let,const**
通常我们不使用var, 而是使用 const 最多,像是数组和对象基本就是使用 const
var 会自动进行作用域提升,污染全局环境带来很多副作用,所以不用

const 特点: 需要初始化,并且值不能被更改, 所以使用 const 定义的叫做常量
let 特点:可以不用初始化,


**减号**
```js
let a = 1,
  b = '2';

console.log(a + b); // '12'
console.log(a - b); //-1
```
因为字符串连接和数字运算都是依靠+号, 而数字运算需要先转换成相同类型,所以计算机选择最简单的方法(字符串连接)
而减号 - 只有一个用处就是数字相减


# callback
回调函数是一种在 JavaScript 中常见的编程模式。它是一个作为参数传递给另一个函数的函数，然后在那个函数内部被调用，或者在适当的时候被执行
**回调函数的运行环境是它被调用时候的环境,所以它可以获取到被调用时候的上下文**
## 数组方法中的回调
```js
 const array = [1, 3, 4, 5, 7];
 let sum = 0;
array.forEach((item, index, arr) => {
  sum += item;
});
```
对数组进行求和,回调函数的运行环境是它被调用时候的环境,所以它可以获取到被调用时候的上下文
所以
```js
(item, index, arr) => {
  sum += item;
}
```
这个回调函数可以获得 forEach 内部执行遍历 array 时候的环境,即(item, index, arr)

==这个回调函数会被数组中的每个元素调用一次。==


## 异步操作
回调也常常用来处理异步,在 JavaScript 中，许多操作是异步的，例如网络请求、定时器、事件监听等。这些操作可能需要一些时间才能完成，而在它们完成之前，我们并不希望阻塞程序的其他部分。这时，我们就可以使用回调函数。

**当异步操作完成时，回调函数会被调用，这样我们就可以在回调函数中处理异步操作的结果**。这种方式允许我们的代码在等待异步操作完成的同时，继续执行其他任务。
```js
setTimeout(()=>{
   console.log('2')
},1000)
consoloe.log('1')
```
比如这段代码中会先打印 1,然后再打印 2

系统执行到异步代码的时候,系统会将它挂起,等待同步代码执行完毕之后再执行异步代码
- 这块涉及的底层其实是事件轮询, 也就是同步和异步代码执行的顺序的,以后再深入

```js
setTimeout(() => {
  console.log('1'); // 处理异步操作的结果
}, 0);

console.log('4');

setTimeout(() => {
  console.log('2'); // 处理异步操作的结果
}, 1000);

console.log('5');

const fn = () => {
  console.log('3'); // 处理异步操作的结果
};

setTimeout(fn, 0); 

// 4 5 1 3 2
```
![[draw/setTimeout|setTimeout]]


# this


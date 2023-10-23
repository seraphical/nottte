# this
- this 是一个使用在 作用域内的关键字
## 全局作用域
this指向window
```js

			function show(){
				alert(this);
			}
			show();
>object Window

```
全局的方法是属于window对象的
等同于下面的函数
```js
    window.show = function(){
            alert(this);
    }
```


## 函数内部
不看函数定义在哪, 不看函数怎么定义, 只看函数的调用方式(箭头函数除外)
### 普通调用
> 函数名( )

严格模式指向 undefined, 非严格模式指向 window

### 对象调用
> 对象名.函数名( )

this 指向 对象( 点前面是谁就是谁)

### 定时器调用,promise,回调函数
>setTimeout(函数, 数字)
 setIterval(函数, 数字)

回调函数中的 this,严格模式指向 undefined, 非严格模式指向 window

```js
          setTimeout(function(){
            console.log(this)  //window
          },2000)

        new Promise(function(resolve,reject){
            console.log(this);   //window
            resolve();
        }).then(function(){
            console.log(this)   //window
        })
```

### 事件处理函数
```js
oDiv.onclick = function(){    alert(this);  };
```
此时就相当于给oDiv这个对象创建了一个方法, this的指向就是当前这个方法(onclick)属于的对象oDiv
this指向**事件源**


### 自调用函数
> `(function( ){ })( )`

相当于在全局执行,this指向window


### 箭头函数
>( )=>{ }

箭头函数内没有this, 箭头函数的this就是外部作用域的this
- 定时器中不使用箭头函数, 其中的this指向window
- 定时器中使用箭头函数, 其中的this指向定时器上一层的this

```js
        var fn=( )=>{
            console.log(this) //window
        }

        document.addEventListener("click",fn); 
```




## call,apply,bind
作用:强行改变 this 指向,不管你本身指向哪里, 我让你指向谁你就得指向谁


### call和 apply
#### call
- 语法: 
    - 函数名.call( )
    - 对象名.函数名.call( )
- 参数:
    - 第一个参数: 该函数本次调用时函数内的this指向
    - 第二个参数开始: 依次是该函数的每一个实参
- 特点: 立即调用函数

#### apply
- 语法: 
    - 函数名.apply( )
    - 对象名.函数名.apply( )
- 参数
    - 第一个参数: 该函数本次调用时函数内的this指向
    - 第二个参数: 是一个数组或者伪数组数据类型都行, 内部的每一个数据依次是该函数的实参
- 特点: 立即调用函数
- 特殊作用: 改变函数传递参数的方式
    - Math.max.apply(null, arr)

#### 区别
传参方式, call 将按参数顺序从第二个参数开始填入,apply 只有两个参数, 第二个参数是一个数组, 参数都写在数组中


#### 传入不同参数时候的表现
1.  数字
    - 传入数字 1 的时候, 指向数值对象
    - 严格模式的时候 , 传入什么指向什么

2.  不传参
    - 没有传入时, 指向 window
    - 严格模式时, 指向 undefined

3.  null
    - 传入 null 时, 指向 window
    - 严格模式下指向 null


### bind
- 语法
    - 函数名.bind( )
    - 对象名.函数名.bind( )
- 参数: 
    - 第一个参数: 该函数本次调用时函数内的this指向
    - 第二个参数开始: 依次是该函数的每一个实参
- 特点:
    - 不会立即调用函数, 而是返回一个新的函数
    - 一个和原先一模一样的函数, 只是被锁定了this
- 特殊作用
    - 修改一些不需要立即执行的函数的this指向
    - 例如: 事件处理函数, 定时器处理函数

```js
     function handler() {
            console.log(this);
        }
        // //指向 window
        div.addEventListener('click', handler.bind())
```



# 类的创建方式
## 原始模式
```js
 const jack = {};
jack.name = 'jack';
 jack.age = 10;
 jack.study = function () {
   console.log('study');
 };

 const rose = {};
 rose.name = 'rose';
rose.age = 10;
 rose.study = function () {
  console.log('study');
 };

```

## 工厂模式
```js
function Student(name) {
  const obj = {}; // 原料
  obj.name = name;
  obj.age = 10;
  obj.study = () => {
    console.log('study');
  }; // 加工
  return obj; // 出厂
}
//工厂模式
const jack = Student('jack');
const rose = Student('rose');
```
用函数解决代码重复的问题,但是函数依然存了两份

## 构造函数
为了解决从原型对象生成实例的问题, js 提供了一个构造函数模式.
同时提供了 this 变量和 new 运算符.对构造函数使用 new 运算符,就能够使 this 绑定在实例对象上.
```js
function Student(name) {
  this.name = name;
  this.age = 10;
  this.study = () => {
    console.log('study');
  };
}
```

**构造函数的一些重要概念**
 1. 和 new 关键字连用
    ※ 构造函数其实就是函数
    ※  只不过在调用的时候, 和 new 关键字连用了
    ※ 所以函数内会自动创建并返回一个对象数据类型
    ※ 并且函数内的 this 指向本次创建出来的对象
    ※ 注意: ==如果不和 new 关键字连用, 那么不会自动创建并返回对象数据类型==

  2. 建议首字母大写
    ※ 就是为了和其他函数做一个区分
    ※  看到函数名就知道调用的时候应 该和 new 关键字连用
    ※ 回忆内置构造函数
        ※  new Object
        ※  new Array
        ※  new Data
        ※  new RegExp
        ※  new XMLHttpRequest
        ※  new Promise

  3. 构造函数内不要书写 return
    ※  ==因为构造函数会自动返回本次创建出来的对象==
    ※  如果你 return 了一个基本数据类型, 写了白写
    ※  如果你 return 了一个复杂数据类型, 构造函数白写

  4. 构造函数内的 this 指向
    ※  因为函数在调用的时候和 new 关键字连用了
    ※  所以函数内的 this 指向本次自动创建出来的对象
    ※  我们管这个自动创建出来的对象叫做 实例对象
    ※  我们管这个创建对象的过程叫做 实例化 的过程
    ※  注意: 箭头函数绝对不能当做构造函数使用

### 构造函数模式模式的问题
构造函数很好用, 但是缺点是浪费内存. 
在构造函数中, study方法是相同的, 这就会造成每生成一个实例都会产生重复的内容
```js
console.log(jack.study === rose.study); //false
```
那么能不能只让重复的东西只产生一次呢, 然后所有的实例都指向那个内存地址?


## prototype 模式
每一个构造函数都有一个prototype属性, 指向另一个对象. 这个对象的所有属性和方法都会被构造函数的实例实现
作用:为了解决方法书写在构造函数体内而造成的资源浪费
### 原型
1. 每一个函数天生自带一个属性, 叫做prototype,是一个对象数据类型
2. 每一个对象天生自带一个属性, 叫做`_ _proto _ _`,  指向所属构造函数的prototype
3. 当你访问一个对象的成员( 属性和方法 )的时候
    - 首先在对象自己本身查找, 如果有直接使用, 停止查找
    - 如果没有, 会自动去到自己的 `_ _proto _ _` 查找, 如果有直接使用, 停止查找


### 构造函数的 prototype
```js
function Student(name) {
  this.name = name;
  this.age = 10;

}
Student.prototype.write = () => {
  console.log('write');
};
const jack = new Student('jack'); //! new 了一个构造函数,创建了一个实例 对象, Student 的实例,实例是实现构造函数的
const rose = new Student('rose');
console.log(jack.write === rose.write); //true
```


## prototype 模式的验证方法

### isPrototypeOf( )
使用这个方法来判断原型对象和实例之间的关系
```js

		alert(Student.prototype.isPrototypeOf(jack));
>true

```

### hasOwnProperty( )
每个实例对象都有一个hasOwnProperty( )方法,用于判断某一个属性是本地属性还是继承自原型对象的属性
```js

			alert(jack.hasOwnProperty('name'));
>true

```

### in 运算符
1. 用来判断某个实例是否含有某个属性, ==不管是不是本地属性==
```js

			alert('name' in jack);
>true
```


# es6的类语法
```js
 class Student{
     constructor(){}
     study(){

     }
 }
```
底层就是上面的 prototype 形式, study 其实是被定义在 Student 的 prototype 上的


# 继承
- 继承出现在两个构造函数之间的关系
- 书写构造函数的时候
    - 属性书写在构造函数体内
    - 方法书写在构造函数原型
- @ 目的: 让子类的实例可以使用父类的属性和方法


- 常见继承方案( ES6以前)
    - 原型继承
    - 借用继承
    - 组合继承
    - 拷贝继承
    - 寄生继承
    - 寄生式组合继承


```js
function Person(name, age) {
  this.name = {
    firstName: name,
  };
  this.age = age;
}
Person.prototype.play = () => {
  console.log('i can play');
};

function Student() {}
```
目的:让 Student 的实例能够拥有 Person 的方法和属性

## 原型继承
```js
const jack = new Person('jack', 18);
Student.prototype = jack;
const xiaoming = new Student();
const xiaohong = new Student();
xiaoming.name.firstName = 'wangxiaoming';
console.log(xiaoming.name);
console.log(xiaohong.name);
```
优点:
- 可以继承父类构造函数的方法;
- 可以继承父类构造函数的属性;
缺点: 
- 不能够自己初始化属性;
- 引用类型的属性会被所有实例共享



# 作业(周三或者周四交就行,先着重看项目)
做一个选项卡
![[link/Pasted image 20231023164107.png]]
比如上面这三项(可以不用看样式), 被选中的项背景变红, 点击属性,属性背景变红,点击项目,项目的背景变红. 三个里面同时只有一个能被选中哦

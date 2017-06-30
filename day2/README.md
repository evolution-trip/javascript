# javascript

## Day 2 数组和for

### 数组
#### 什么是数组？

> 通俗的说数据就是一堆类似的东西。
> 不通俗的说，数组就是相同数据类型的元素按一定顺序排列的集合。
> 例如： 张三 李四 王五 赵六 孙七 周八 吴九 郑十
> 或者：Sunday Monday Tuesday Wednesday Thursday Friday Saturday
> 或者：1 2 4 8 16 32 64 128

#### 数组有些什么特点？
1. 类型相同（javascript中允许不相同）
2. 长度
3. 有顺序

#### 在Javascript中如何声明数组
在Javascript中可以使用`Array`和 `new`关键字创建一个数组，也可以使用`[]`方括号，创建一个数组。
```javascript
	var a1=new Array(); //无参构造函数，创建一空数组。
	var a2=new Array(5);// 一个数字参数构造函数，指定数组长度,创建指定长度的数组
	var a3 = [];//使用方括号，创建空数组
	var a4=[10]; //使用中括号，并传入初始化数据
```
#### 使用数组
##### 长度
```javascript

	var a1 = new Array();
	console.log(a1);
	console.log(a1.length);

	var a2 = new Array(5);
	console.log(a2);
	console.log(a2.length);

	var a3 = [];
	console.log(a3);
	console.log(a3.length);

	var a4 = [10];
	console.log(a4.length);
	console.log(a4);

```
##### push和pop
`push`是向Array的末位添加若干元素，`pop`则是把末位最后一个元素删除掉。

```javascript
var arr = [1,2];
console.log(arr.length);
console.log(arr);
arr.push(3);//向arr的末位增加一个元素 3
console.log(arr.length);
console.log(arr);
arr.pop();//删除arr末位元素
console.log(arr);
console.log(arr.length);
```
其实数组还有很多方法，可以自己学习。

### for循环

#### for循环是干嘛的？
`for` 是javascript的一个关键字，如果你想一遍又一遍的执行相同的代码，并且每次执行的结果不同，那么使用`for`就很方便。
例如：从打印1到10。
#### 例子
```javascript
//普通写法：
	console.log(1);
	console.log(2);
	console.log(3);
	console.log(4);
	console.log(5);
	console.log(6);
	console.log(7);
	console.log(8);
	console.log(9);
	console.log(10);
	//OK，完成了，很简单对不对。代码简单，逻辑清楚。


	//那如果打印1到100，是不是要复制粘贴十次，再挨个该数字。其实也行，累就累点，也是能实现。
	//那如果打印1到1000000呢？是不是感觉有些吃不消了。
	//这个时候 for作用就体现出来了。

	//for的写法：
	for(var i = 1;i<=100;i++){//想打印多少次，就把对应的数字改为多少。
      console.log(i);
	}
```
#### for循环的语法
```javascript
	for(语句 1; 语句 2; 语句 3){
       被执行的代码块
	}
	//语句 1 （代码块）开始前执行 starts.
	//语句 2 定义运行循环（代码块）的条件
	//语句 3 在循环（代码块）已被执行之后执行
	for(var i=0;i<10;i++){
      console.log(i)
	}
```

#### 当for循环遇到数组
在有些情况下，我们需要将一个数组里所有的元素都取出来，这时就可以使用for语句。
 ```javascript
    var cars = new Array();
    cars[0] = "BMW";
    cars[1] = "Benz";
    cars[2] = "Ford";
    cars[3] = "Volkswagen";

    for(var i=0;i<cars.length;i++){
        console.log(cars[i]);
    }

 ```


### 练习

#### 使用for循环语句，求出数组中所有数字的总和。
```javascript
	var items = [1,23,4,5,6,7,8,9,0,1,3,22,10086];
	//请问items数组中所有的数字加起来是多少，请使用for循环求出该值。
```
#### 使用for循环语句，找出数组中最小的数字是谁。

```javascript
	var items = [1,23,4,5,6,7,8,9,0,1,3,22,10086,-1,-1008];
	//请找出items数组中最小的是谁。
	//提示：使用for语句和if语句。
```

#### 完成练习后，请将练习文件通过git命令上传到github.com中。

```shell
	// 更新本地代码库
	git pull origin master 
	git add 你的文件
	//提交本地代码
	git commit -m "home work" .
	//提交代码到远程代码库
	git push origin master
```
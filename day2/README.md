# javascript

## Day 2 数组和for

### 数组
####什么是数组？

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


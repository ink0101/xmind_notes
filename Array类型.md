## Array 类型方法整理

### 总览

![Array类型.png](./assets/Array类型.png)

### 数组的特殊性
和其他语言相比，JavaScript 中数组的特殊性在于：

* 数组的每一项都可以保存任意类型的数据。
* 数组的 length 属性不仅可读，而且可写。
	* 读  
	
	* 写  
	
		通过设置 length 值，可以从数组的末尾移除项或向数组中添加新项
		
		```
		const arr1 = [1,2,3];
		arr1.length = 1; // [1]
		arr1.length = 3; // [1, empty × 2]
		```


### 方法介绍

方法根据功能大概分为以下几类：

#### 创建方法

##### ES5

1. 构造函数

```
// new 关键字可以省略

const arr1 = new Array(); // []

// 注：给构造函数传递一个参数的时候，会根据参数的类型，有不同的行为
const arr2 = new Array(3); // [empty × 3] 注意这里每一项的值是空
const arr3 = new Array('3'); // ['3']

const arr4 = new Array('m', 'n'); // ["m", "n"]
```

2. 数组字面量

```
const arr1 = ['m', 'm'];
```

##### ES6

1. from
2. of

#### 检测数组

确定某个对象是不是数组的经典问题：

参阅： [检测数组方法](https://www.w3cplus.com/javascript/array-part-2.html)

1. instanceof

	```
	if (value instance of Array) {
		// 对数组执行某些操作
	}
	```
	instanceof 操作符可以用来判断某个构造函数的 prototype 属性是否存在另外一个要检测对象的原型链上。也就是判断instanceof前面的对象是否是后面的类或对象的实例。
	
	前提： 假设存在单一的全局环境。
	
	问题： 不同的全局执行环境可能存在不同版本的Array构造函数。

2. isArray
	
	ES5原生支持的方法，确定某个值是否是数组。
	
	问题： 低版本浏览器不支持。
	
#### 转换方法

1. toString
2. toLocalString
3. valueOf
4. join

##### ES6 
1. 扩展运算符 `...`

#### 栈方法

1. push
2. pop

#### 队列方法

1. shift
2. unshift

#### 重排序方法

1. reserve
2. sort

#### 操作方法

1. concat
2. slice
3. splice

##### ES6 

1. copyWithin
2. fill

#### 位置方法

1. indexOf
2. lastIndexOf

#### 迭代方法

1. every
2. some
3. filter
4. map
5. forEach

##### ES6

1. find
2. findIndex
3. entries
4. keys
5. values

#### 缩小方法

1. reduce
2. rediceRight



### 参考链接
[JavaScript学习笔记：检测数组方法](https://www.w3cplus.com/javascript/array-part-2.html)
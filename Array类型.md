## Array 类型方法整理

### 总览

![Array类型.png](./assets/Array类型.png)

### 数组的特殊性
和其他语言相比，JavaScript 中数组的特殊性在于：

* 数组的每一项都可以保存任意类型的数据。
* 数组的 length 属性不仅可读，而且可写。


### 方法介绍

方法根据功能大概分为以下几类：

#### 创建方法

##### ES5

1. 构造函数
2. 数组字面量

##### ES6

1. from
2. of

#### 检测数组

1. instanceof
2. isArray

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


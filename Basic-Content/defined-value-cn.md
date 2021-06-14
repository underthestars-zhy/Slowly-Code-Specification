# 定义量值

> 基本类型大部分与Swift用法完全一样

## 定义变量

通过`var`关键词定义**变量**。

```slowly
var value = 1
print(value) // 1
value = 2
print(value) // 2
```

## 定义常量

通过`let`关键词定义**常量**。

```slowly
let value = 1
print(value) // 1
value = 2 // 错误行为
```

## 快速定义

通过`:=`关键词进行**快速定义**。
当变量名称**全大写**的时候默认定义**常量**，当**非全大写**默认定义变量。
快速定义无法**显示**指定类型。

```slowly
value := 1 // 定义变量
value1: Int := 2 // 错误行为
MAX_INT := 3 // 定义常量
```
# 起点和终点

> Slowly有着健全的代码管理机制

## 基本组成

在Slowly中，**项目**是基本组成部分。一个项目就是一个**文件夹**，内部包含多个**Slowly相关文件**。在编译的时候我们运行的是一个项目而不是单个文件。

```bash
- Project
	- main.slowly
	- Other File
		- class.slowly
	- __slowly__
		- __package__.json
```

## 起点

为了在项目中识别哪个是代码的开始文件，我们引入了**起点**概念。
在代码开始处标上`@main`象征这个是代码开端。
一个项目只有**一个**起点。
我们会在项目中所有文件挨个搜索。

```slowly
import Slowly
// something...
func hi() {}
// something..
@mian
a := "hello, i'm slowly"
print(a)
```

使用起点能**加快编译速度**。

## 终点

终点代码代码的最终处，可以不加，默认文件最后一行为终点。
使用`@end`标记终点。

```slowly
a := "hi"
print(a)
// @end
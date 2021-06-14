# Start and end

> Slowly has a sound code management mechanism

## basic component

In Slowly, the **project** is the basic component. A project is a **folder**, which contains multiple **Slowly related files**. When compiling, we are running a project instead of a single file.

```bash
-Project
	-main.slowly
	-Other File
		-class.slowly
	-__slowly__
		-__package__.json
```

## Starting point

In order to identify which is the start file of the code in the project, we introduced the concept of **starting point**.
Mark `@main` at the beginning of the code to signify that this is the beginning of the code.
There is only **one** starting point for a project.
We will search all files in the project one by one.

```slowly
import Slowly
// something...
func hi() {}
// something..
@mian
a := "hello, i'm slowly"
print(a)
```

Use the starting point to **speed up compilation**.

## End

The end point of the end point code code can be omitted, and the end point is the default line at the end of the file.
Use `@end` to mark the end point.

```slowly
a := "hi"
print(a)
// @end
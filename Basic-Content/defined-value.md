# Define the quantity value

> Most of the basic types are exactly the same as Swift usages.

## Define variables

Define **variate** by `var` keyword.

```slowly
var value = 1
print(value) // 1
value = 2
print(value) // 2
```

## Define constants

Define **constant** by `let` keyword.

```slowly
let value = 1
print(value) // 1
value = 2 // Wrong behavior
```

## Quick definition

**Quickly define** by `:=` keyword.

When the variable name **is fully capitalized**, the default definition of **constant** is defined, and when **non-full capitalization** defaults the variable is defined.

Quick definition cannot **display** specify type.

```slowly
value := 1 // Define variables
value1: Int := 2 // Wrong Behavior
MAX_INT := 3 // DEFINE CONSTANT
```
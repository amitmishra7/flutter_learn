# Functions

* Function is a set of statements that take inputs, do some specific computation and produces output.
* Functions are created when certain statements are repeatedly occurring in the program and a function is created to replace them.
* Functions make it easy to divide the complex program into smaller sub-groups and increase the code reusability of the program.

## Syntax

```
return_type function_name ( parameters ) {
   // Body of function
   return value;
}
```

In above syntax
* **function_name** defines the name of the function.
* **return_type** defines the datatype in which output is going to come.
* **return value** defines the value to be returned from the function.

```
function_name (argument_list);
```

In above syntax
* **function_name** defines the name of the function.
* **argument_list** is the list of the parameter that the function requires.

### Functions with return types 

```
bool isFunctional(){
    return true;
}
```

### Functions without return types 

```
void add(int a, int b){
    print(a+b);
}
```

### Functions with different parameter types

|Sr.No.| Parameter | Description | 
|------|-----------|-------------|
|   1. | Optional Positional Parameter |To specify it use square (‘[ ]’) brackets|
|2.| Optional Named parameter | To specify it use curly(‘{ }’) brackets. Paramter name should be written while passing its values|
|3.|Optional parameter with default values | Here parameters are assign with default values. |     |

**Optional Positional Parameter**

```
void gfg1(int g1, [ var g2 ])
{
    // Creating function 1
    print("g1 is $g1");
    print("g2 is $g2");
}
```

**Optional Named Parameter**

```
void gfg2(int g1, { var g2, var g3 })
{
    // Creating function 1
    print("g1 is $g1");
    print("g2 is $g2");
    print("g3 is $g3");
}
```

**Optional parameter with default values**

```
void gfg3(int g1, { int g2 : 12 })
{
    // Creating function 1
    print("g1 is $g1");
    print("g2 is $g2");
}
```

```
void main()
{
    // Calling the function with optional parameter
    gfg1(01);
 
    // Calling the function with Optional Named parameter
    gfg2(01, g3 : 12);
 
    // Calling function with default valued parameter

    gfg3(01);
}
```

### Recursive Functions in Dart

The recursive function is those functions in which function calls itself.

```
/// Computes the nth Fibonacci number.
int fibonacci(int n)
{
    // This is recursive function as it calls itself
    return n < 2 ? n : (fibonacci(n - 1) + fibonacci(n - 2));
}
```

### Lambda Function in Dart

The Lambda Function can only have one expression but can take any number of arguments

```
void add(int a, int b) => a + b;
```





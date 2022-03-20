## DataTypes

__Fundamental Data Types__

int  
float  
bool  
str  
list  
tuple  
set  
dict  

__Classes -> custom types__

__Specialized Data Types__

None

## Python program to find pip version

```python
from importlib import metadata

print("Pip Version : ",metadata.version("pip"))
pip_metadata = metadata.metadata("pip")
print(list(pip_metadata))
print("Homepage: ",pip_metadata["Home-page"])
print("Python requirements",pip_metadata["Requires-Python"])
```

## Python code to check data type and math

```python
print(type(2 + 4))
print(type(2 - 4))
print(type(2 * 4))
print(type(2 / 4))
print(type(10.56))
print(2 ** 3) # 2 power of 3
print(2 // 4) # double division
print(5 // 4) # double division
print(6 % 4) # Modulo
```

## Math functions

```python
#math functions
print(round(3.1))
```

|Function|Description|
|---|---|
|`ceil(x)`        |`Returns the smallest integer greater than or equal to x.`|
|`copysign(x, y)` |`Returns x with the sign of y`|
|`fabs(x)`	       |`Returnsthe absolute value of x`|
|`factorial(x)`   |`Returns the factorial of x`|
|`floor(x)`	   |`Returns the largest integer less than or equal to x`|
|`fmod(x, y)`	   |`Returns the remainder when x is divided by y`|
|`frexp(x)`	   |`Returns the mantissa and exponent of x as the pair (m, e)`|
|`fsum(iterable)` |`Returns an accurate floating point sum of values in the iterable`|
|`isfinite(x)`	   |`Returns True if x is neither an infinity nor a NaN (Not a Number)`|
|`isinf(x)`   |`Returns True if x is a positive or negative infinity`|
|`isnan(x)`	   |`Returns True if x is a NaN`|
|`ldexp(x, i)`	   |`Returns x * (2**i)`|
|`modf(x)`	       |`Returns the fractional and integer parts of x`|
|`trunc(x)`	   |`Returns the truncated integer value of x`|
|`exp(x)`	       |`Returns e**x`|
|`expm1(x)`	   |`Returns e**x - 1`|
|`log(x[, b])`	   |`Returns the logarithm of x to the base b (defaults to e)`|
|`log1p(x)`	   |`Returns the natural logarithm of 1+x`|
|`log2(x)`	       |`Returns the base-2 logarithm of x`|
|`log10(x)`	   |`Returns the base-10 logarithm of x`|
|`pow(x, y)`	   |`Returns x raised to the power y`|
|`sqrt(x)`	       |`Returns the square root of x`|
|`acos(x)`	       |`Returns the arc cosine of x`|
|`asin(x)`	       |`Returns the arc sine of x`|
|`atan(x)`	       |`Returns the arc tangent of x`|
|`atan2(y, x)`	   |`Returns atan(y / x)`|
|`cos(x)`	       |`Returns the cosine of x`|
|`hypot(x, y)`	   |`Returns the Euclidean norm, sqrt(x*x + y*y)`|
|`sin(x)`	       |`Returns the sine of x`|
|`tan(x)`	       |`Returns the tangent of x`|
|`degrees(x)`	   |`Converts angle x from radians to degrees`|
|`radians(x)`	   |`Converts angle x from degrees to radians`|
|`acosh(x)`	   |`Returns the inverse hyperbolic cosine of x`|
|`asinh(x)`	   |`Returns the inverse hyperbolic sine of x`|
|`atanh(x)`	   |`Returns the inverse hyperbolic tangent of x`|
|`cosh(x)`	       |`Returns the hyperbolic cosine of x`|
|`sinh(x)`	       |`Returns the hyperbolic cosine of x`|
|`tanh(x)`	       |`Returns the hyperbolic tangent of x`|
|`erf(x)`	       |`Returns the error function at x`|
|`erfc(x)`	       |`Returns the complementary error function at x`|
|`gamma(x)`	   |`Returns the Gamma function at x`|
|`lgamma(x)`	   |`Returns the natural logarithm of the absolute value of the Gamma function at x`|
|`pi`	           |`Mathematical constant, the ratio of circumference of a circle to it's diameter (3.14159...)`|
|`e`           |`mathematical constant e (2.71828...)`|

## Operator Precedence

```python
# Operator Precedence

print(20 - 3 * 4) #8

print((20 - 3) + 2 ** 2) #21

#()
# **
# * /
# + -
```

## bin()

```python
#bin

print(bin(5))
print(int('0b101', 2))


# Python3 program for implementation
# of int() function
num = 13
 
String = '187'
 
# Stores the result value of
# binary "187" and num addition
result_1 = int(String) + num
print("int('187') + 13 = ", result_1, "\n")
 
# Example_2
str = '100'
 
print("int('100') with base 2 = ", int(str, 2))
print("int('100') with base 4 = ", int(str, 4))
print("int('100') with base 8 = ", int(str, 8))
print("int('100') with base 16 = ", int(str, 16))

#Convert binary string to Python int base
# "111" taken as the binary string
binaryString = "111"
 
# Stores the equivalent decimal
# value of binary "111"
Decimal = int(binaryString, 2)
 
print("Decimal equivalent of binary 111 is", Decimal)
 
# "101" taken as the octal string
octalString = "101"
 
# Stores the equivalent decimal
# value of binary "101"
Octal = int(octalString, 8)
 
print("Decimal equivalent of octal 101 is", Octal)
```

## python keywords

|Keyword|Description|
|---|---|
|`and`	       |`A logical operator`|
|`as`	       |`To create an alias`|
|`assert`	   |`For debugging`|
|`break`	   |`To break out of a loop`|
|`class`	   |`To define a class`|
|`continue`	|`To continue to the next iteration of a loop`|
|`def`	        |`To define a function`|
|`del`	        |`To delete an object`|
|`elif`	    |`Used in conditional statements, same as else if`|
|`else`	    |`Used in conditional statements`|
|`except`	    |`Used with exceptions, what to do when an exception occurs`|
|`False`	    |`Boolean value, result of comparison operations`|
|`finally`	    |`Used with exceptions, a block of code that will be executed no matter if there is an exception or not`|
|`for`	        |`To create a for loop`|
|`from`	    |`To import specific parts of a module`|
|`global`	    |`To declare a global variable`|
|`if`	        |`To make a conditional statement`|
|`import`	    |`To import a module`|
|`in`	        |`To check if a value is present in a list, tuple, etc.`|
|`is`	        |`To test if two variables are equal`|
|`lambda`	    |`To create an anonymous function`|
|`None`	    |`Represents a null value`|
|`nonlocal`	|`To declare a non-local variable`|
|`not`	        |`A logical operator`|
|`or`	        |`A logical operator`|
|`pass`	    |`A null statement, a statement that will do nothing`|
|`raise`	    |`To raise an exception`|
|`return`	    |`To exit a function and return a value`|
|`True`	    |`Boolean value, result of comparison operations`|
|`try`	        |`To make a try...except statement`|
|`while`	    |`To create a while loop`|
|`with`	    |`Used to simplify exception handling`|
|`yield`	    |`To end a function, returns a generator`|
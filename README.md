

# PHP
PHP is a server scripting language, and a powerful tool for making dynamic and interactive Web pages.

## PHP Introduction

**What is PHP?**
-   PHP is an acronym for "PHP: Hypertext Preprocessor"
-   PHP is a widely-used, open source scripting language
-   PHP scripts are executed on the server
-   PHP is free to download and use

**What is a PHP File?**
-   PHP files can contain text, HTML, CSS, JavaScript, and PHP code
-   PHP code is executed on the server, and the result is returned to the browser as plain HTML
-   PHP files have extension "`.php`"

 **Why PHP?**
-   PHP runs on various platforms (Windows, Linux, Unix, Mac OS X, etc.)
-   PHP is compatible with almost all servers used today (Apache, IIS, Nginx.)
-   PHP supports a wide range of databases
-   PHP is free. Download it from the official PHP resource:  [www.php.net](http://www.php.net/)
-   PHP is easy to learn and runs efficiently on the server side

**PHP is an amazing and popular language!**
It is powerful enough to be at the core of the biggest blogging system on the web (WordPress)!  
It is deep enough to run the largest social network (Facebook)!  
It is also easy enough to be a beginner's first server side language!

**PHP  Installation**
The official PHP website (PHP.net) has installation instructions for PHP:  [http://php.net/manual/en/install.php](http://php.net/manual/en/install.php)

## PHP Syntax

A PHP script can be placed any where in the document.
A PHP script starts with  `<?php`  and ends with  `?>`:

```php
<?php
// PHP code goes here  
?>
```
The default file extension for PHP files is "`.php`".

**PHP Case Sensitivity**
```php
<?php  
ECHO  "Hello World! \n";  
echo  "Hello World! \n";  
EcHo  "Hello World! \n";  
?>
```
## PHP  Comments
A comment in PHP code is a line that is not executed as a part of the program. Its only purpose is to be read by someone who is looking at the code.

Syntax for single-line comments:
```php
<?php  
// This is a single-line comment  
  
# This is also a single-line comment  
?>
```

Syntax for multiple-line comments:
```php
<?php  
/*  
This is a multiple-lines comment block  
that spans over multiple  
lines  
*/  
?>
```

## PHP  Variables

In PHP, a variable starts with the  `$`  sign, followed by the name of the variable:
```php
$txt = "Hello world!";  
$x = 5;  
$y = 10.5;  
```

A variable can have a short name (like x and y) or a more descriptive name (age, carname, total_volume).

Rules for PHP variables:

-   A variable starts with the  `$`  sign, followed by the name of the variable
-   A variable name must start with a letter or the underscore character
-   A variable name cannot start with a number
-   A variable name can only contain alpha-numeric characters and underscores (A-z, 0-9, and _ )
-   Variable names are case-sensitive (`$age`  and  `$AGE`  are two different variables)

**Output Variables**
The PHP  `echo`  statement is often used to output data to the screen.
```php
$txt = "W3Schools.com";  
echo  "I love $txt!";  
```
The following example will produce the same output as the example above:
```php
$txt = "W3Schools.com";  
echo  "I love " . $txt . "!";  
```
The following example will output the sum of two variables:
```php
$x = 5;  
$y = 4;  
echo $x + $y;  
```
**PHP is a Loosely Typed Language**
In the example above, notice that we did not have to tell PHP which data type the variable is.
PHP automatically associates a data type to the variable, depending on its value. Since the data types are not set in a strict sense, you can do things like adding a string to an integer without causing an error.

**The PHP echo Statement**
The  `echo`  statement can be used with or without parentheses:  `echo`  or  `echo()`.

```php
echo  "PHP is Fun! \n";  
echo  "Hello world! \n";  
echo  "I'm about to learn PHP! \n";  
echo  "This ", "string ", "was ", "made ", "with multiple parameters.";  
```
**The PHP print Statement**
The  `print`  statement can be used with or without parentheses:  `print`  or  `print()`.

```php
print  "PHP is Fun! \n";  
print  "Hello world! \n";  
print  "I'm about to learn PHP!";  
```

## PHP Data Types
Variables can store data of different types, and different data types can do different things.

PHP supports the following data types:

-   String
-   Integer
-   Float (floating point numbers - also called double)
-   Boolean
-   Array
-   Object
-   NULL
-   Resource

**PHP String**
A string is a sequence of characters, like "Hello world!".
A string can be any text inside quotes. You can use single or double quotes:
```php
$x = "Hello world!";  
$y = 'Hello world!';  
  
echo $x;  
echo  "<br>";  
echo $y;  
```
**PHP Integer**
An integer data type is a non-decimal number between -2,147,483,648 and 2,147,483,647.

Rules for integers:

-   An integer must have at least one digit
-   An integer must not have a decimal point
-   An integer can be either positive or negative
-   Integers can be specified in: decimal (base 10), hexadecimal (base 16), octal (base 8), or binary (base 2) notation

In the following example $x is an integer. The PHP var_dump() function returns the data type and value:
```php
$x = 5985;  
var_dump($x);  
```
**PHP Float**
A float (floating point number) is a number with a decimal point or a number in exponential form.
In the following example $x is a float. The PHP var_dump() function returns the data type and value:
```php
$x = 10.365;  
var_dump($x);  
```
**PHP Boolean**
A Boolean represents two possible states: TRUE or FALSE.
```php
$x = true;  
$y = false;
```
**PHP Array**
An array stores multiple values in one single variable.
In the following example $cars is an array. The PHP var_dump() function returns the data type and value:
```php
$cars = array("Volvo","BMW","Toyota");  
var_dump($cars);  
```
**PHP Object**
Classes and objects are the two main aspects of object-oriented programming.
A class is a template for objects, and an object is an instance of a class.

**PHP NULL Value**
Null is a special data type which can have only one value: NULL.
A variable of data type NULL is a variable that has no value assigned to it.
Variables can also be emptied by setting the value to NULL:
```php
$x = "Hello world!";  
$x = null;  
var_dump($x);  
```

## PHP String Functions
In this chapter we will look at some commonly used functions to manipulate strings.

**Return the Length of a String**
The PHP  `strlen()`  function returns the length of a string.
```php
echo strlen("Gitmag website!"); // outputs 15  
```
**Count Words in a String**
The PHP  `str_word_count()`  function counts the number of words in a string.
```php
echo str_word_count("Gitmag website!"); // outputs 2  
```
**Reverse a String**
The PHP  `strrev()`  function reverses a string.
```php
echo strrev("Gitmag website!"); // outputs !etisbew gamtiG  
```
**Search For a Text Within a String**
The PHP  `strpos()`  function searches for a specific text within a string. If a match is found, the function returns the character position of the first match. If no match is found, it will return FALSE.
```php
echo strpos("Gitmag website!", "website"); // outputs 7  
```
**Replace Text Within a String**
The PHP  `str_replace()`  function replaces some characters with some other characters in a string.
```php
echo str_replace("website", "academy", "Gitmag website"); // outputs Gitmag academy!
```
## PHP Numbers
One thing to notice about PHP is that it provides automatic data type conversion.
So, if you assign an integer value to a variable, the type of that variable will automatically be an integer. Then, if you assign a string to the same variable, the type will change to a string.

This automatic conversion can sometimes break your code.

**PHP Integers**
PHP has the following functions to check if the type of a variable is integer:
-   is_int()
-   is_integer() - alias of is_int()
-   is_long() - alias of is_int()
```php
$x = 5985;  
var_dump(is_int($x));  
  
$x = 59.85;  
var_dump(is_int($x));  
```
**PHP Floats**
A float is a number with a decimal point or a number in exponential form.
PHP has the following functions to check if the type of a variable is float:
-   is_float()
-   is_double() - alias of is_float()
```php
$x = 10.365;  
var_dump(is_float($x));
```
**PHP Numerical Strings**
The PHP is_numeric() function can be used to find whether a variable is numeric. The function returns true if the variable is a number or a numeric string, false otherwise.
```php
$x = 5985;  
var_dump(is_numeric($x));  
  
$x = "5985";  
var_dump(is_numeric($x));  
  
$x = "59.85" + 100;  
var_dump(is_numeric($x));  
  
$x = "Hello";  
var_dump(is_numeric($x));
```
**PHP Casting Strings and Floats to Integers**
Sometimes you need to cast a numerical value into another data type.
The (int), (integer), or intval() function are often used to convert a value to an integer.
```php
// Cast float to int  
$x = 23465.768;  
$int_cast = (int)$x;  
echo $int_cast;  
  
echo  "\n";  
  
// Cast string to int  
$x = "23465.768";  
$int_cast = (int)$x;  
echo $int_cast;
```

## PHP Math
PHP has a set of math functions that allows you to perform mathematical tasks on numbers.

**PHP pi() Function**
The  `pi()`  function returns the value of PI:
```php
echo(pi()); // returns 3.1415926535898
```
**PHP min() and max() Functions**
The  `min()`  and  `max()`  functions can be used to find the lowest or highest value in a list of arguments:
```php
echo(min(0, 150, 30, 20, -8, -200)); // returns -200  
echo(max(0, 150, 30, 20, -8, -200)); // returns 150
```
**PHP abs() Function**
The  `abs()`  function returns the absolute (positive) value of a number:
```php
echo(abs(-6.7)); // returns 6.7
```
**PHP sqrt() Function**
The  `sqrt()`  function returns the square root of a number:
```php
echo(sqrt(64)); // returns 8
```
**PHP round() Function**
The  `round()`  function rounds a floating-point number to its nearest integer:
```php
echo(round(0.60)); // returns 1  
echo(round(0.49)); // returns 0
```
**Random Numbers**
The  `rand()`  function generates a random number:
```php
echo(rand());
```
For example, if you want a random integer between 10 and 100 (inclusive), use  `rand(10, 100)`:
```php
echo(rand(10, 100));
```

## PHP Constants

A constant is an identifier (name) for a simple value. The value cannot be changed during the script.
A valid constant name starts with a letter or underscore (no $ sign before the constant name).

To create a constant, use the  `define()`  function.

    define(name, value)

Parameters:
-  name: Specifies the name of the constant
-  value: Specifies the value of the constant
```php
define("GITMAG", "Welcome to gitmag.ir!");  
echo GITMAG;
```
**PHP Constant Arrays**
In PHP7, you can create an Array constant using the  `define()`  function.
```php
define("cars", [  
    "Benz",  
    "BMW",  
    "Toyota"  
]);  

var_dump(cars);
```

## PHP Operators
Operators are used to perform operations on variables and values.

PHP divides the operators in the following groups:
-   Arithmetic operators
-   Assignment operators
-   Comparison operators
-   Increment/Decrement operators
-   Logical operators
-   String operators
-   Array operators
-   Conditional assignment operators

**PHP Arithmetic Operators**
The PHP arithmetic operators are used with numeric values to perform common arithmetical operations, such as addition, subtraction, multiplication etc.

Sum of $x and $y
```php
$x = 10;  
$y = 6;
echo $x + $y;
```
Difference of $x and $y
```php
$x = 10;  
$y = 6;
echo $x - $y;
```
Product of $x and $y
```php
$x = 10;  
$y = 6;
echo $x * $y;
```
Quotient of $x and $y
```php
$x = 10;  
$y = 6;
echo $x / $y;
```
Remainder of $x divided by $y
```php
$x = 10;  
$y = 6;
echo $x % $y;
```
Result of raising $x to the $y'th power
```php
$x = 10;  
$y = 3;
echo $x ** $y;
```

**PHP Assignment Operators**
The PHP assignment operators are used with numeric values to write a value to a variable.
The basic assignment operator in PHP is "=". It means that the left operand gets set to the value of the assignment expression on the right.

The left operand gets set to the value of the expression on the right
```php
$x = 10;  
echo $x;
```
Addition
```php
$x = 20;  
$x += 100;
echo $x;
```
Subtraction
```php
$x = 50;
$x -= 30;
echo $x;
```
Multiplication
```php
$x = 5;
$x *= 6;
echo $x;
```
Division
```php
$x = 10;
$x /= 5;
echo $x;
```
Modulus
```php
$x = 15;
$x %= 4;
echo $x;
```
**PHP Comparison Operators**
The PHP comparison operators are used to compare two values (number or string):

Returns true if $x is equal to $y
```php
$x = 100;  
$y = 100;
var_dump($x == $y);

$x = 100;  
$y = "100";
var_dump($x == $y); // returns true because values are equal
```
Returns true if $x is equal to $y, and they are of the same type
```php
$x = 100;  
$y = "100";
var_dump($x === $y); // returns false because types are not equal
```
Returns true if $x is not equal to $y
```php
$x = 100;  
$y = 100;
var_dump($x != $y);

$x = 100;  
$y = "100";
var_dump($x != $y); // returns false because values are equal
```
Returns true if $x is not equal to $y
```php
$x = 100;  
$y = "100";
var_dump($x <> $y); // returns false because values are equal
```
Returns true if $x is not equal to $y, or they are not of the same type
```php
$x = 100;  
$y = "100";
var_dump($x !== $y); // returns true because types are not equal
```
Returns true if $x is greater than $y
```php
$x = 100;
$y = 50;
var_dump($x > $y); // returns true because $x is greater than $y
```
Returns true if $x is less than $y
```php
$x = 10;
$y = 50;
var_dump($x < $y); // returns true because $x is less than $y
```
Returns true if $x is greater than or equal to $y
```php
$x = 50;
$y = 50;
var_dump($x >= $y); // returns true because $x is greater than or equal to $y
```
Returns true if $x is less than or equal to $y
```php
$x = 50;
$y = 50;
var_dump($x <= $y); // returns true because $x is less than or equal to $y
```
**PHP Increment / Decrement Operators**
The PHP increment operators are used to increment a variable's value.
The PHP decrement operators are used to decrement a variable's value.

Increments $x by one, then returns $x
```php
$x = 10;  
echo ++$x;
```
Returns $x, then increments $x by one
```php
$x = 10;  
echo $x++;
```
Decrements $x by one, then returns $x
```php
$x = 10;  
echo --$x;
```
Returns $x, then decrements $x by one
```php
$x = 10;  
echo $x--;
```
**PHP Logical Operators**
The PHP logical operators are used to combine conditional statements.

True if both $x and $y are true
```php
$x = 100;  
$y = 50;
var_dump($x == 100 and $y == 50)
```
True if either $x or $y is true
```php
$x = 100;  
$y = 50;
var_dump($x == 100 or $y == 80)
```
True if either $x or $y is true, but not both
```php
$x = 100;  
$y = 50;
var_dump($x == 100 xor $y == 80)
```
True if both $x and $y are true
```php
$x = 100;  
$y = 50;
var_dump($x == 100 && $y == 50)
```
True if either $x or $y is true
```php
$x = 100;  
$y = 50;
var_dump($x == 100 || $y == 80)
```
True if $x is not true
```php
$x = true;  
var_dump(!$x) 
```

**PHP String Operators**
PHP has two operators that are specially designed for strings.

Concatenation of $txt1 and $txt2
```php
$txt1 = "Gitmag";
$txt2 = " website!";
echo $txt1 . $txt2;
```
Appends $txt2 to $txt1
```php
$txt1 = "Gitmag";
$txt2 = " website!";
$txt1 .= $txt2;
echo $txt1;
```
**PHP Conditional Assignment Operators**
Returns the value of $x.  
The value of $x is _expr2_ if _expr1_ = TRUE.  
The value of $x is _expr3_ if _expr1_ = FALSE
```php
   // if empty($user) = TRUE, set $status = "anonymous"
   $status = (isset($user)) ? "user is exist" : "user is not exist";
   echo $status;
   $user = "Sohrab azinfar";
   // if empty($user) = FALSE, set $status = "logged in"
   echo $status = (isset($user)) ? $user : "user is not exist";
```
Returns the value of $x.  
The value of $x is _expr1_ if _expr1_ exists, and is not NULL.  
If _expr1_ does not exist, or is NULL, the value of $x is _expr2_.  
Introduced in PHP 7
```php
   // variable $user is the value of $_GET['user']
   // and 'anonymous' if it does not exist
   echo $user = $user ?? "anonymous";
  
   // variable $color is "red" if $color does not exist or is null
   echo $color = $color ?? "red";
```

## PHP  Arrays

An array is a special variable, which can hold more than one value at a time.
If you have a list of items (a list of car names, for example), storing the cars in single variables could look like this:
```php
$cars1 = "Volvo";  
$cars2 = "BMW";  
$cars3 = "Toyota";
```
However, what if you want to loop through the cars and find a specific one? And what if you had not 3 cars, but 300?
The solution is to create an array!
An array can hold many values under a single name, and you can access the values by referring to an index number.

**Create an Array in PHP**
In PHP, the  `array()`  function is used to create an array:
```php
array();
```
In PHP, there are three types of arrays:
-   **Indexed arrays**  - Arrays with a numeric index
-   **Associative arrays**  - Arrays with named keys
-   **Multidimensional arrays**  - Arrays containing one or more arrays

**PHP Indexed Arrays**
There are two ways to create indexed arrays:
The index can be assigned automatically (index always starts at 0), like this:
```php
$cars = array("Volvo", "BMW", "Toyota");
```
or the index can be assigned manually:
```php
$cars[0] = "Volvo";  
$cars[1] = "BMW";  
$cars[2] = "Toyota";
```
The following example creates an indexed array named $cars, assigns three elements to it, and then prints a text containing the array values:
```php
$cars = array("Volvo", "BMW", "Toyota");  
echo  "I like " . $cars[0] . ", " . $cars[1] . " and " . $cars[2] . ".";
```
**PHP Associative Arrays**
Associative arrays are arrays that use named keys that you assign to them.
There are two ways to create an associative array:
```php
$age = array("Peter"=>"35", "Ben"=>"37", "Joe"=>"43");
```
```php
$age['Peter'] = "35";  
$age['Ben'] = "37";  
$age['Joe'] = "43";
```
The named keys can then be used in a script:
```php
$age = array("Peter"=>"35", "Ben"=>"37", "Joe"=>"43");  
echo  "Peter is " . $age['Peter'] . " years old.";
```
**PHP - Multidimensional Arrays**
A multidimensional array is an array containing one or more arrays.
PHP supports multidimensional arrays that are two, three, four, five, or more levels deep. However, arrays more than three levels deep are hard to manage for most people.

**PHP - Two-dimensional Arrays**
```php
$cars = array (  
    array("Volvo",22,18),  
    array("BMW",15,13),  
    array("Saab",5,2),  
    array("Land Rover",17,15)  
);
```
Now the two-dimensional $cars array contains four arrays, and it has two indices: row and column.
To get access to the elements of the $cars array we must point to the two indices (row and column):
```php
echo $cars[0][0].": In stock: ".$cars[0][1].", sold: ".$cars[0][2];
```

**Get The Length of an Array - The count() Function**
The  `count()`  function is used to return the length (the number of elements) of an array:
```php
$cars = array("Volvo", "BMW", "Toyota");  
echo count($cars);
```
**PHP  in_array()  Function**
Check if the "Volvo" exists in an array:
```php
$cars = array("Volvo", "BMW", "Toyota");  
var_dump(in_array("Volvo", $cars))
```
**PHP  array_key_exists()  Function**
Check if the key "Peter" exists in an array:
```php
$age = array("Peter"=>"35", "Ben"=>"37", "Joe"=>"43");  
var_dump(array_key_exists("Peter", $age))
```
**PHP  array_keys()  Function**
Return an array containing the keys:
```php
$age = array("Peter"=>"35", "Ben"=>"37", "Joe"=>"43");  
var_dump(array_keys($age))
```
**PHP  array_reverse()  Function**
Return an array in the reverse order:
```php
$cars = array("Volvo", "BMW", "Toyota");  
var_dump(array_reverse($cars))
```
**PHP  array_slice()  Function**
```php
$colors = ["red","green","blue","yellow","brown"];  
var_dump(array_slice($colors, 2));
```

**PHP Array Operators**
The PHP array operators are used to compare arrays.

Union of $x and $y
```php
$x = array("a" => "red", "b" => "green");  
$y = array("c" => "blue", "d" => "yellow");  
var_dump($x + $y); // union of $x and $y
```
Returns true if $x and $y have the same key/value pairs
```php
$x = array("a" => "red", "b" => "green");  
$y = array("c" => "blue", "d" => "yellow");  
var_dump($x == $y);
```
Returns true if $x and $y have the same key/value pairs in the same order and of the same types
```php
$x = array("a" => "red", "b" => "green");  
$y = array("b" => "green", "a" => "red");  
var_dump($x === $y);
```
Returns true if $x is not equal to $y
```php
$x = array("a" => "red", "b" => "green");  
$y = array("c" => "blue", "d" => "yellow");  
var_dump($x != $y);
```
Returns true if $x is not equal to $y
```php
$x = array("a" => "red", "b" => "green");  
$y = array("c" => "blue", "d" => "yellow");  
var_dump($x <> $y);
```
Returns true if $x is not identical to $y
```php
$x = array("a" => "red", "b" => "green");  
$y = array("a" => "red", "b" => "green"); 
var_dump($x !== $y);
```

## PHP Conditional Statements
Very often when you write code, you want to perform different actions for different conditions. You can use conditional statements in your code to do this.

In PHP we have the following conditional statements:

-   `if`  statement - executes some code if one condition is true
-   `if...else`  statement - executes some code if a condition is true and another code if that condition is false
-   `if...elseif...else`  statement - executes different codes for more than two conditions
-   `switch`  statement - selects one of many blocks of code to be executed

**PHP - The if Statement**
The  `if`  statement executes some code if one condition is true.
```php
if (condition) {
    code to be executed if condition is true;  
}
```
```php
$t = 15;  
if ($t < 20) {  
    echo  "Have a good day!";  
}
```

**PHP - The if...else Statement**
The  `if...else`  statement executes some code if a condition is true and another code if that condition is false.
```php
if (condition) {  
    code to be executed if condition is true;
} else {  
    code to be executed if condition is false;  
}
```
```php
$t = 10;  
if ($t < 20) {  
   echo  "Have a good day!";  
} else {  
   echo  "Have a good night!";  
}
```

**PHP - The if...elseif...else Statement**
The  `if...elseif...else`  statement executes different codes for more than two conditions.
```php
if (condition) {  
    code to be executed if this condition is true;  
} elseif (condition) {  
    code to be executed if first condition is false and this condition is true;  
...
} else {  
    code to be executed if all conditions are false;  
}
```
```php
$t = 8;    
if ($t < 10) {  
    echo  "Have a good morning!";  
} elseif ($t < 20) {  
    echo  "Have a good day!";  
} else {  
    echo  "Have a good night!";  
}
```
**The PHP switch Statement**
The  `switch`  statement is used to perform different actions based on different conditions.
Use the  `switch`  statement to  **select one of many blocks of code to be executed**.
```php
switch (n) {  
    case label1: 
        code to be executed if n=label1;
        break;  
    case label2:  
        code to be executed if n=label2;
        break;  
    case label3:  
        code to be executed if n=label3;
        break;  
        ...  
    default:  
	_code to be executed if n is different from all labels;
}
```
```php
$favcolor = "red";  
switch ($favcolor)  {  
    case  "red":  
	echo  "Your favorite color is red!";  
	break;  
    case  "blue":  
	echo  "Your favorite color is blue!";  
	break;  
    case  "green":  
	echo  "Your favorite color is green!";  
	break;  
    default:  
	echo  "Your favorite color is neither red, blue, nor green!";  
}
```

## PHP Loops
Often when you write code, you want the same block of code to run over and over again a certain number of times. So, instead of adding several almost equal code-lines in a script, we can use loops.

Loops are used to execute the same block of code again and again, as long as a certain condition is true.

In PHP, we have the following loop types:
-   `while`  - loops through a block of code as long as the specified condition is true
-   `do...while`  - loops through a block of code once, and then repeats the loop as long as the specified condition is true
-   `for`  - loops through a block of code a specified number of times
-   `foreach`  - loops through a block of code for each element in an array

**The PHP while Loop**
The  `while`  loop executes a block of code as long as the specified condition is *true*.
```php
while (condition is true) {  
    code to be executed;  
}
```
```php
$x = 1;   
while($x <= 5) {  
    echo  "The number is: $x \n";  
    $x++;  
}
```
```php
$x = 0;  
while($x <= 100) {  
    echo  "The number is: $x \n";  
    $x+=10;  
}
```
**The PHP do...while Loop**
The  `do...while`  loop will always execute the block of code once, it will then check the condition, and repeat the loop while the specified condition is true.
```php
do {  
    code to be executed;  
} while (condition is true);
```
```php
$x = 1;  
do {  
   echo  "The number is: $x \n";  
   $x++;  
} while ($x <= 5);
```
**The PHP for Loop**
The  `for`  loop is used when you know in advance how many times the script should run.
```php
for (init counter; test counter; increment counter) {  
    code to be executed for each iteration;
}
```
Parameters:

-   _init counter_: Initialize the loop counter value
-   _test counter_: Evaluated for each loop iteration. If it evaluates to TRUE, the loop continues. If it evaluates to FALSE, the loop ends.
-   _increment counter_: Increases the loop counter value

```php
for ($x = 0; $x <= 10; $x++)  {  
    echo  "The number is: $x \n";  
}
```
```php
for ($x = 0; $x <= 100; $x+=10)  {  
    echo  "The number is: $x \n";  
}
```
**The PHP foreach Loop**
The  `foreach`  loop works only on arrays, and is used to loop through each key/value pair in an array.
```php
foreach ($array as  $value) {  
    code to be executed; 
}
```
```php
$colors = array("red", "green", "blue", "yellow");  
foreach ($colors as $value) {  
    echo  "$value \n";  
}
```
```php
$age = array("Peter"=>"35", "Ben"=>"37", "Joe"=>"43");  
foreach($age as $value) {  
    echo  "$value \n";  
}
```
**Loop Through an Associative Array**
To loop through and print all the values of an associative array, you could use a  `foreach`  loop, like this:
```php
$age = array("Peter"=>"35", "Ben"=>"37", "Joe"=>"43");  
  
foreach($age as $x => $x_value) {  
   echo  "Key=" . $x . ", Value=" . $x_value . "\n";  
}
```

**PHP Break**
You have already seen the  `break`  statement used in an earlier chapter of this tutorial. It was used to "jump out" of a  `switch`  statement.
The  `break`  statement can also be used to jump out of a loop.
This example jumps out of the loop when  **x**  is equal to  **4**:
```php
for ($x = 0; $x < 10; $x++) {  
    if ($x == 4) {  
        break;  
    }  
    echo  "The number is: $x \n";  
}
```
**Break and Continue in While Loop**
You can also use  `break`  and  `continue`  in  `while`  loops:
```php
$x = 0;  
while($x < 10) {  
    if ($x == 4) {  
	break;  
    }  
    echo  "The number is: $x \n";  
    $x++;  
}
```
```php
$x = 0;  
while($x < 10) {  
    if ($x == 4) {  
	$x++;  
        continue;  
    }  
    echo  "The number is: $x \n";  
    $x++;  
}
```

## PHP Built-in Functions

PHP has over 1000 built-in functions that can be called directly, from within a script, to perform a specific task.
Please check out our PHP reference for a complete overview of the  [PHP built-in functions](https://www.w3schools.com/php/php_ref_overview.asp).

## PHP User Defined Functions

Besides the built-in PHP functions, it is possible to create your own functions.

-   A function is a block of statements that can be used repeatedly in a program.
-   A function will not execute automatically when a page loads.
-   A function will be executed by a call to the function.

**Create a User Defined Function in PHP**
A user-defined function declaration starts with the word  `function`:
```php
function functionName() 
{  
    code to be executed;  
}
```
```php
function writeMsg() 
{  
    echo  "Hello world!";  
}  
  
writeMsg(); // call the function
```
**PHP Function Arguments**
Information can be passed to functions through arguments. An argument is just like a variable.

Arguments are specified after the function name, inside the parentheses. You can add as many arguments as you want, just separate them with a comma.

The following example has a function with one argument ($fname). When the familyName() function is called, we also pass along a name (e.g. Jani), and the name is used inside the function, which outputs several different first names, but an equal last name:
```php
function familyName($fname) 
{  
    echo  "$fname Refsnes. \n";  
}  
  
familyName("Jani");  
familyName("Hege");  
familyName("Stale");  
familyName("Kai Jim");  
familyName("Borge");
```
The following example has a function with two arguments ($fname and $year):
```php
function familyName($fname, $year) 
{  
    echo  "$fname Refsnes. Born in $year \n";  
}  
  
familyName("Hege", "1975");  
familyName("Stale", "1978");  
familyName("Kai Jim", "1983");
```
**PHP is a Loosely Typed Language**
In the example above, notice that we did not have to tell PHP which data type the variable is.

PHP automatically associates a data type to the variable, depending on its value. Since the data types are not set in a strict sense, you can do things like adding a string to an integer without causing an error.

In PHP 7, type declarations were added. This gives us an option to specify the expected data type when declaring a function, and by adding the  `strict`  declaration, it will throw a "Fatal Error" if the data type mismatches.

```php
function addNumbers(int $a, int $b) 
{  
    echo$a + $b;  
}  

addNumbers(5, "5 days");  
// since strict is NOT enabled "5 days" is changed to int(5), and it will return 10
```
**PHP Default Argument Value**
The following example shows how to use a default parameter. If we call the function setHeight() without arguments it takes the default value as argument:
```php
function setHeight(int $minheight = 50) 
{  
    echo  "The height is : $minheight \n";  
}  
  
setHeight(350);  
setHeight(); // will use the default value of 50  
setHeight(135);  
setHeight(80);
```
**PHP Functions - Returning values**
To let a function return a value, use the  `return`  statement:
```php
function sum(int $x, int $y) 
{  
    $z = $x + $y;  
    return $z;  
}  
  
echo  "5 + 10 = " . sum(5, 10) . "\n";  
echo  "7 + 13 = " . sum(7, 13) . "\n";  
echo  "2 + 4 = " . sum(2, 4);
```
**PHP Return Type Declarations**
PHP 7 also supports Type Declarations for the  `return`  statement. Like with the type declaration for function arguments, by enabling the strict requirement, it will throw a "Fatal Error" on a type mismatch.

To declare a type for the function return, add a colon (  `:`  ) and the type right before the opening curly (  `{`  )bracket when declaring the function.
```php
function addNumbers(float $a, float $b) : float 
{  
    return $a + $b;  
}  
echo addNumbers(1.2, 5.2);
```
You can specify a different return type, than the argument types, but make sure the return is the correct type:
```php
function addNumbers(float $a, float $b) : int {  
    return (int)($a + $b);  
}  
echo addNumbers(1.2, 5.2);
```

## PHP  Global Variables  - Superglobals
Some predefined variables in PHP are "superglobals", which means that they are always accessible, regardless of scope - and you can access them from any function, class or file without having to do anything special.

The PHP superglobal variables are:
-   $GLOBALS
-   $_SERVER
-   $_REQUEST
-   $_POST
-   $_GET
-   $_FILES
-   $_ENV
-   $_COOKIE
-   $_SESSION

**PHP $GLOBALS**
$GLOBALS is a PHP super global variable which is used to access global variables from anywhere in the PHP script (also from within functions or methods).
PHP stores all global variables in an array called $GLOBALS[_index_]. The  _index_  holds the name of the variable.
The example below shows how to use the super global variable $GLOBALS:
```php
$x = 75;  
$y = 25;  
  
function addition() {  
    $GLOBALS['z'] = $GLOBALS['x'] + $GLOBALS['y'];  
}  
  
addition();  
echo $z;
```
**PHP $_SERVER**
$_SERVER is a PHP super global variable which holds information about headers, paths, and script locations.
The example below shows how to use some of the elements in $_SERVER:
```php
var_dump($_SERVER)
```
**PHP $_REQUEST**
PHP $_REQUEST is a PHP super global variable which is used to collect data after submitting an HTML form.

The example below shows a form with an input field and a submit button. When a user submits the data by clicking on "Submit", the form data is sent to the file specified in the action attribute of the <form> tag. In this example, we point to this file itself for processing form data. If you wish to use another PHP file to process form data, replace that with the filename of your choice. Then, we can use the super global variable $_REQUEST to collect the value of the input field:

```php
<html>  
<body>  
  
<form method="post"  action="<?php  echo  $_SERVER['PHP_SELF'];?>">  
    Name: <input type="text"  name="fname">  
    <input type="submit">  
</form>  
  
<?php  
if  ($_SERVER["REQUEST_METHOD"] ==  "POST") {  
    // collect value of input field  
    $name =  $_REQUEST['fname'];  
    if  (empty($name)) {  
	echo  "Name is empty";  
    }  else  {  
	echo  $name;  
    }  
}  
?>  

</body>  
</html>
```
**PHP $_POST**
PHP $_POST is a PHP super global variable which is used to collect form data after submitting an HTML form with method="post". $_POST is also widely used to pass variables.

The example below shows a form with an input field and a submit button. When a user submits the data by clicking on "Submit", the form data is sent to the file specified in the action attribute of the <form> tag. In this example, we point to the file itself for processing form data. If you wish to use another PHP file to process form data, replace that with the filename of your choice. Then, we can use the super global variable $_POST to collect the value of the input field:
```php
<html>  
<body>  
  
<form method="post"  action="<?php  echo  $_SERVER['PHP_SELF'];?>">  
    Name: <input type="text"  name="fname">  
    <input type="submit">  
</form>  
  
<?php  
if  ($_SERVER["REQUEST_METHOD"] ==  "POST") {  
    // collect value of input field  
    $name =  $_POST['fname'];  
    if  (empty($name)) {  
	echo  "Name is empty";  
    }  else  {  
	echo  $name;  
    }  
}  
?>  
  
</body>  
</html>
```
**PHP $_GET**
PHP $_GET is a PHP super global variable which is used to collect form data after submitting an HTML form with method="get".
$_GET can also collect data sent in the URL.
Assume we have an HTML page that contains a hyperlink with parameters:
```php
<html>  
<body>  
  
<?php  
echo  "Study "  .  $_GET['subject'] .  " at "  .  $_GET['web'];  
?>  
  
</body>  
</html>
```

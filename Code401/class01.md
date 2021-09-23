#  Java Basics
Java is a programming language and computing platform first released by Sun Microsystems in 1995. There are lots of applications and websites that will not work unless you have Java installed, and more are created every day. Java is fast, secure, and reliable. From laptops to datacenters, game consoles to scientific supercomputers, cell phones to the Internet, Java is everywhere!

Java is a very easy to learn and here are some of java basics:
## Variables: 
Just like any other programming language java uses variables. There are number of variable types in java such as:
1. Instance Variables: Are also called **Non-Static Fields** because their values are unique to each instance of a class. Does not use keyword **static**.
2. Class Variables: Are also called **Static Fields** A class variable is any field declared with the static modifier and it works by telling the compiler that there is exactly one copy of this variable in existence, regardless of how many times the class has been instantiated. These variables are declared by using keywords such as **static and final**.
3. Local Variables: Similar to how an object stores its state in fields, a method will often store its temporary state in local variables. The syntax for declaring a local variable is similar to declaring a field (for example, **int count = 0;**).
4. Parameters: Important to note here is that parameters are always classified as **variables** not **fields**.

## Basic Naming Syntax:
About Java programs, it is very important to keep in mind the following points:
1. Case Sensitivity: Java is case sensitive, which means identifier Hello and hello
.would have different meaning in Java.
2. Class Names: For all class names the first letter should be in Upper Case. If
several words are used to form a name of the class, each inner word's first letter
should be in Upper Case (Pascal syntax).
3. Method Names: All method names should start with a Lower Case letter. If
several words are used to form the name of the method, then each inner word's
first letter should be in Upper Case (Camel case)
4. Variable Names: Are case-sensitive. A variable's name can be any legal identifier an unlimited-length sequence of Unicode letters and digits, beginning with a letter, the dollar sign **$,** or the underscore character **_**.
*Important to note here is that the better practice for variable naming is to name them starting with a letter rather than characters*.

## Primitive Data Types:
There are 8 primitive data types supported by the Java programming language and they are divided into 4 groups:
1. Variables of an integer type (among these are byte, short, int, long).
2. Floating point variables (among these are float, double)
3. Symbols (char)
4. Logic variables (boolean).

## Arrays:
An array is a container object that holds a fixed number of values of a single type. The length of an array is established when the array is created. After creation, its length is fixed.
Each item in an array is called an element, and each element is accessed by its numerical index. Arrays are a powerful and useful concept used in programming. Java SE provides methods to perform some of the most common manipulations related to arrays.

## Operators in Java:
| Operators      | Precedence |
| ----------- | ----------- |
| postfix	  | expr++ expr--
| unary       | ++expr --expr +expr -expr ~ !
| multiplicative | 	* / %
| additive     | + -
| shift     | << >> >>>
| relational     | < > <= >= instanceof
| equality     | 	== !=
| bitwise AND     | 	&
| bitwise exclusive OR     | ^
| bitwise inclusive OR     | |
| logical AND   | &&
| logical OR     | | |
| ternary     | ? :


## Expressions, Statements, and Blocks
expressions are the core components of statements; statements may be grouped into blocks.

### Expressions
is a construct made up of variables, operators, and method invocations, which are constructed according to the syntax of the language, that evaluates to a single value. 
The data type of the value returned by an expression depends on the elements used in the expression.

### Statements
are roughly equivalent to sentences in natural languages. A statement forms a complete unit of execution. 

### Blocks
is a group of zero or more statements between balanced braces and can be used anywhere a single statement is allowed.

## The if-then and if-then-else Statements

### The if-then Statement
is the most basic of all the control flow statements. It tells your program to execute a certain section of code only if a particular test evaluates to true.

### The if-then-else Statement
it provides a secondary path of execution when an "if" clause evaluates to false. 

## The switch Statement
Unlike if-then and if-then-else statements, the switch statement can have a number of possible execution paths. A switch works with the byte, short, char, and int primitive data types.

## The while and do-while Statements
The while statement evaluates expression, which must return a boolean value. If the expression evaluates to true, the while statement executes the statement(s) in the while block. The while statement continues testing the expression and executing its block until the expression evaluates to false.

## Differences between while and do-while loop:
is that do-while evaluates its expression at the bottom of the loop instead of the top but otherwise the while loop

## For Loop
it provides a compact way to iterate over a range of values. Programmers often refer to it as the "for loop" because of the way in which it repeatedly loops until a particular condition is satisfied.

## Branching statements in Java:
There are three branching statements in java:
1. Break Statement: it has two forms labeled and unlabeled. unlabeled is used in switch statement and we can use it to terminate from the for and while loops. 
2. Continue Statement: it skips the current iteration of a for, while , or do-while loop. The unlabeled form skips to the end of the innermost loop's body and evaluates the boolean expression that controls the loop. Whereas the labled skips the current iteration of an outer loop marked with the given label.
3. Return Statement: exits from the current method, and control flow returns to where the method was invoked. The return statement has two forms: one that returns a value, and one that doesn't. To return a value, simply put the value
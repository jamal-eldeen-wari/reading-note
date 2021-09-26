# Java Packages and Import:
What is a package??
A: Is a place where it contains java classes. A package name has the same name as the directory (folder) which contains the .java files.

How to use a package statement ??
The package statement identifies the package that a java program belongs to. If your program does not include a package statement, the program belongs to the default package, which is simply a package that has no name.
This is acceptable for short programs written for testing purposes.

What is imports ??
It allows you to use the built in java classes that are available in the java API

There are three options for imports:
1. The wildcard character (*): is used to specify that all classes with that package are available to your program. This is the most common programming style. ex: import javax.swing.*;
2. Classes can be specified explicitly on import instead of using the wildcard character. ex: import javax.swing.JOptionPane;
3. We can write the fully qualified name without import ex: javax.swing.JOptionPane.showMessageDialog(null, "Hi");

Some Important imports:
1. import java.awt.*;	Common GUI elements.
2. import java.awt.event.*;	The most common GUI event listeners.
3. import javax.swing.*;	More common GUI elements. Note "javax".
4. import java.util.*;	Data structures (Collections), time, Scanner, etc classes.
5. import java.io.*;	Input-output classes.
6. import java.text.*;	Some formatting classes.
7. import java.util.regex.*;	Regular expression classes.

# Loops in Java
The while and do-while Statements:
The while statement evaluates expression, which must return a boolean value. If the expression evaluates to true, the while statement executes the statement(s) in the while block. The while statement continues testing the expression and executing its block until the expression evaluates to false.

For Loop:
it provides a compact way to iterate over a range of values. Programmers often refer to it as the "for loop" because of the way in which it repeatedly loops until a particular condition is satisfied.
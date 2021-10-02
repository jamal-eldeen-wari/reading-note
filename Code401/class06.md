# Inheritance:
Different kinds of objects often have a certain amount in common with each other. Object-oriented programming allows classes to inherit commonly used state and behavior from other classes.
Synatax:
The syntax for creating a subclass is simple. At the beginning of your class declaration, use the extends keyword.

# Interface:
An interface in Java is a blueprint of a class. There can be only abstract methods in the Java interface, not method body. It is used to achieve abstraction and multiple inheritance in Java. In other words, you can say that interfaces can have abstract methods and variables.
In order to implement an interface,we need to use keyword **implements**.

Some important notes about interface:
Interface methods do not have a body - the body is provided by the "implement" class.
On implementation of an interface, you must override all of its methods.
Interface methods are by default abstract and public.
Interface attributes are by default public, static and final.
An interface cannot contain a constructor.

# Package:
A package is a namespace that organizes a set of related classes and interfaces.
The Java platform provides an enormous class library (a set of packages) suitable for use in your own applications. This library is known as the "Application Programming Interface", or "API" for short. Its packages represent the tasks most commonly associated with general-purpose programming.

# Abstract VS Interface:
1. Like abstract classes, interfaces cannot be used to create objects.
2. In terms of speed interface is slow compare to abstract class.
3. We can Implement several Interfaces, but for abstract only one abstract class.
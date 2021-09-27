# Primitives VS Objects:
Java programming language has a two-fold type system consisting of primitives such as int, boolean and reference types such as Integer, Boolean. Every primitive type corresponds to a reference type.
**Very important to note** Every object contains a single value of the corresponding primitive type.
The wrapper classes are immutable once they are declared they cant be changed.
The process of converting a primitive type to a reference one is called **autoboxing**, the opposite process is called **unboxing**.
## What is the pros and cons of primitives and objects:
The decision what object is to be used is based on what application performance we try to achieve, how much available memory we have, the amount of available memory and what default values we should handle.
and below we will show you how primitive data types impact memory:
1. boolean – 1 bit
2. byte – 8 bits
3. short, char – 16 bits
4. int, float – 32 bits
5. long, double – 64 bits
Variables of these types live in the stack and hence are accessed fast.
The reference types are objects, they live on the heap and are relatively slow to access. They have a certain overhead concerning their primitive counterparts.

## Performance:
The performance of a Java code is quite a subtle issue, it depends very much on the hardware on which the code runs, on the compiler that might perform certain optimizations, on the state of the virtual machine, on the activity of other processes in the operating system.

##  Default Values:
Default values of the primitive types are 0. For numeric types, false for the boolean type, \u0000 for the char type. For the wrapper classes, the default value is null.It means that the primitive types may acquire values only from their domains, while the reference types might acquire a value (null) that in some sense doesn't belong to their domains.

## Usage:
As we've seen, the primitive types are much faster and require much less memory. Therefore, we might want to prefer using them.

On the other hand, current Java language specification doesn't allow usage of primitive types in the parametrized types (generics),  in the Java collections or the Reflection API.

# Exceptions:
The Java programming language uses exceptions to handle errors and other exceptional events. This lesson describes when and how to use exceptions.
 is an event that occurs during the execution of a program that disrupts the normal flow of instructions.
 ## Advantages of Exceptions:
 The use of exceptions to manage errors has some advantages over traditional error-management techniques. 

 # Scanning:
 Objects of type Scanner are useful for breaking down formatted input into tokens and translating individual tokens according to their data type.
 Scanning has a simple syntax first it starts with an import **import java.util.Scanner;** 



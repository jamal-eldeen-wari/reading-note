# Objects In Java:
Real-world objects share two characteristics: They all have state and behavior and they are similar to software objects. An object stores its state in fields (variables in some programming languages) and exposes its behavior through methods (functions in some programming languages). Methods operate on an object's internal state and serve as the primary mechanism for object-to-object communication.

What are the benefits of bundling code into individual software objects??
A: 
1. Modularity:The source code for an object can be written and maintained independently of the source code for other objects. Once created, an object can be easily passed around inside the system.
2. Information-hiding:  By interacting only with an object's methods, the details of its internal implementation remain hidden from the outside world.
3. Code re-usability: If an object already exists you can use that object in your program. This allows specialists to implement/test/debug complex, task-specific objects, which you can then trust to run in your own code.
4. Pluggability and debugging ease: If a particular object turns out to be problematic, you can simply remove it from your application and plug in a different object as its replacement.

# Classes In Java: 
 A class is the blueprint from which individual objects are created.

 Class declaration: The class has a body between the curly braces contains all the code that provides for the life cycle of the objects created from the class such as initializing new objects, declarations for the fields that provide the state of the class and its objects, and methods to implement the behavior of the class and its objects.
 Java allows you to put an access modifirer in the beggingin of the class declaration

 ### Declaring Member variables:
 There are three kinds of variables:
 1. Member variables in a class—these are called fields.
 2. Variables in a method or block of code—these are called local variables.
 3. Variables in method declarations—these are called parameters.

 ### Access Modifiers:
 The first (left-most) modifier used lets you control what other classes have access to a member field.
 Two most popular AM are:
 1. Public modifier—the field is accessible from all classes.
 2. Private modifier—the field is accessible only within its own class.

 ### Constructors:
 A class contains constructors that are invoked to create objects from the class blueprint.There is a default one that is called empty constructor and there are constructors that you can create.

 


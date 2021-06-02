# Order Of Execution:
It is the order that the statements will be executed one by one.
# Execution Contexts:
It is used by javascript interpreter where every statement in a script lives in one of three execution contexts:
 1. GLOBAL CONTEXT: It is the code that is in the script not in function.**THERE IS ONLY ONE GLOBAL CONTEXT IN ANY PAGE**.
 2. FUNCTION CONTEXT: It is the code that is being running within a function.**EACH FUNCTION HAS ITS OWN FUNCTION CONTEXT**.
 3. EVAL CONTEXT: It is the text that is being executed that is similar to the code in a internal function**CALLED EVAL()**

# Variable Scope:
It is the first  two execution contexts correspond with the notion of scope:
 * GLOBAL SCOPE: If a variable is declared outside a function, it can be used anywhere because it has global scope.
 ### Function Level Scope: 
 When a variable is declared within a function, it can only be used within that function. This is because it has function-level scope.

# Stack: 
The way javascript interpreter works is by proccessing one line of code at a time. When a statement needs data from another function it **STACKS** the new function on top of the current task.

# Execution Context and Hoisting:
Each time a script enters a new execution context, there are two phases 
of activity:
 1. Prepare: 
  * Thr new scope is created.
  * Variables, functions, and arguments are created. 
  * The value of the this keyword is determined.
 2. Execute: 
  * Now it can assign values to variables.
  * Reference functions and run their code.
  * Execute statements.

**Hoisting:** It gives you the ability to call function before declaration and assign value to a variable that has not yet been declared. This is because any variables and functions within each execution context are created before they are executed.

**VIP** is that each execution context also creates its own *variable object*. This object contains details of all 
of the variables, functions, and parameters for that execution context.

# Scope in javascript:
Each execution context has its own va ri ables object. It holds the variables, functions, and parameters available within it. Each execution context can also access its parent's variables object. Functions in js are known as **lexical scope** 

# Errors in javascript:
If a JavaScript statement generates an error, then it throws an **exception**. When it reaches this point it stops and looks for the execption handling code. If you are anticipating that something in your code may cause an error, you can use a set of statements to handle the error. This is important because if the error is not handled, 
the script will just stop processing and the user will not know why. So exception-handling code should inform users when there is a problem.

# Error Object:
It can help us to find where our mistakes are and browsers have tools to help you read them. Error objects has some properties:
 1. name: Type of execution
 2. message: Description
 3. fileNumber: Name of the javascript file.
 4. lineNumber: Line number of error.

 ## Types of Errors in javascript:
 1. Error:  It is a Generic error the other errors are all based upon this error.
 2. Syntax Error: Syntax has not been followed.
 3. ReferenceError: Tried to reference a variable that is not declared/within scope.
 4. TypeError: An unexpected data type that cannot be coerced.
 6. Range Error: Numbers not in acceptable range.
 7. URI Error: encodeURI ().decodeURI(),and similar methods used incorrectly.
 8. EvalError: eval() function used incorrectly.

 **Important to note** that NAN is not an error.

 How can we deal with error??
 A: Actually there is two ways to deal with an error:
  1. Debug the script to fix an error: Is to track down the source of the error, and fix it. 
  2. Handeling errors gracefully: This can be done by using try catch statements, throw and finally statements.

## Debugging Tips:
Below will be some debugging tips that will helps us figure out our errors:
1. Use another browser.
2. Adding numbers to the console
3. Stripping down code to the minimum you need.
4. Find someone to expalin your code to.
5. Search for the error online you might find someone stuck on the same error or close to your error.

## Common Errors:
1. Go back to basics of javascript because javascript is a sensitive language.
2. Missed characters or added characters to your code that made your faulty.
3. Data type issues.    
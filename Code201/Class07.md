# Domain Modeling:
It is a process of creating a conceptual model in code for specific problem. Sometimes the model can describe various entities, attributes, behaviour and also constraints that govern the problem domain. 

# Table: 
It represents information in a grid format, the advantage of using grid is taht it allows us to understand the complex data by referencing on two axes.

What is a table cell?
A: where each block in the grid is refered to as table cell 
**To write a table in HTML we write row by row.**

## Some Basic table structure:
Some important tags for table :
1. table tag: is used to create a table in HTML which is written row by row in HTML.
2. tr tag: Which indicates the start of each row using the openning tr tag. This tag is usually followed by one or more elements.
3. td tag: Each cell of a table is represented using a td tag. Where some browsers draw lines around tables.
4. th tag: It os similar to the td tag but the only difference is its purpose is to represent the heading for either a column or a row. it is useful for table heading.
**VIP** One of the most important feature for the th tag is it helps people who use screen readers, improves the ability for search engines to index your pages, and also enables you to control the appearance of tables better 
when you start to use CSS.  

## Spanning Columns:
It is done by using this attribute **Colspan** where it can be used in either th tag or td tag, and it indicates how many columns that cell should run across. So the **colspan =3** attribute it indicates that the cell should run across three columns.

## Spanning Row:
It is done by using this attribute **rowspan** where it can be used in either th tag or td tag it is the oppesite of the colspan.


## Long Tables: 
There are three elements that help to distinguish between the main content of the table and the first and last rows.
These elements help people who use screen readers and also allow you to style these sections in a different manner than the rest of the table.

Those three elements are : 
1. thread tag: any heading for the table should be inside the thread tag.
2. tbody tag: The body of the table must sit inside this tag.
3. tfoot tag: It is used for the footer.

# Javascript:
Two ways to create an object either using Constructor Notation or Object Literals.
## Constructors Notation:
Creating an object using constructor notation it is done by using the keyword **new** and the object constructor create a blank object where you can properties and methods to the project, normally constructors are used to define a template of something for example:
let games = new Object();
where games here is an instance of that object.

**Important to note** that if we want to create an empty object using literals notation for instance: 
let games = {}; empty braces creates an empty object.

### Updating object:
To update an object it can be done by using either dot notation or square brackets.
**dot Notation:** games.add  = 'FIFA'
**Square Brackets:** games['add'] = 'FIFA'.

## Deleting Object: 
Two Ways to delete an object:
1. By using delete keyword for example delete games.name;
2. By making the that property equals to an empty string for example: games.name  = '';

## Creating many objects:
Javascript provides us the ability to have multiple objects where the the object constructors can use a function as a template for creating an object.

**This keyword:** It used instead of an object name to indicate that the property or method belongs to the object.
**Some Important Notes:**
 * Each statement inside the constructor is seperated by semicolon rather than a colon in objects.
 * The name of the constructor function usually begins in capital letters unlike functions where it starts with lower case letters.
 * The benefit of the uppercase used in constructors is to remind the developer to use **new keyword** when they create an object.

Now to access the constructor function we use instances these instances are normal variables but they are known as object when they are used with constructors.

when exactly can we use constructors??
A:  When we have a very complex object that needs to be available but not being used.

## Arrays: 
Arrays are special type of objects where they hold a related set of **key/value** pair just like an object but the key for each value is indexed if you want to access it, it can only happen using indexes.

**VIP** Combining Arrays and Objects we can create a complex data structure.Where the Arrays can store a series of objects and Objects can also hold arrays.

## Three groups of built in objects:
Those three groups each one of them porvides a set of tools that can be used to write scripts for web page.

1. Browser Object Model:
It creates a model of the browser tab or window. The top most object is the **window** object which represents the current browser window or tab.

2. Document Object Model: Creates a model of the current webpage. The topmost object is **document** which represent the page as a whole.

3. Global Javascript Objects: 
They are group of individual objects that relate to different parts of javascript language. The names of global objects usually starts with capital letter.
# Programming Deficulties:
One of the hardest part in programming is trying to understand the problem that occurs in your screen especially new programmer. And also talking about defficulty in programming there is also something that is called problem domain. one of the ways to to reduce the problem domain is :
 *  Using a familiar problem: a problem that can be easily understood for beginners 

**Important to note** that programming is easy if you understand the problem domain by trying to make the problem domain easier to understand by by cutting out cases and narrowing your focus to a particular part of the problem. To do that affectively you need to shrink your work or cut the problem into subproblem understanding sub problems is much eaiser than taking the whole problem and try to understand it as a whole which will make your life misrable.

One of the most important note that the writer mentioned is that talking to customer who knows about the problem domain is a waste of time 

# Object Literals:
There are two important concepts in objects that we need to keep in mind is that:
 1. In Objects Variable are known as **Property**.
 2. In Objects Functions are known as **Methods**.

 **VIP** Objects represents the properties and the methods as key/value pairs.

 An easy way to create an object by using Objects Literals:
 Ex :

 var nameOne = {


     name: 'Something',

     age: 30,

     doAnything: function(){

         return anything



     }

 };

 Objects store its content as key/value pair

 **Accessing objects** is done by using the dot notation or by using square brackets for example:
 
 **Using dot notation**:

 var nameFirst = nameOne.name;

 **Using Square Brackets**:

 var nameFirst = nameOne [ 'name' ];

 # Document Object Model: 
 It is known as DOM, once the web browser loads the web page it creates a modle of that page and that model is known as **DOM Tree**. That tree is stored in browsers memory and it consists of four main types of nodes:

  1. THE DOCUMENT NODE: When you access any element, attribute, or text node, you navigate to it via the document node. It is the starting point for all visits to the **DOM tree**. 
  2. ELEMENT NODES: To access the DOM tree, you start by looking for elements. Once you find the element you want, then you can access its text and attribute nodes if you want to.
  3. ATTRIBUTE NODES: are not children of the element thar carries them; they are part of that element. Once you   access an element, there are specific JavaScript methods and properties to read or change that element's attributes.
  4. TEXT NODES: Once we access the element then we can reach the text within that element. Same as Attribute node text nodes cannot have children.

To access and update the DOM tree it requires two steps:
 1. Locate the node that represents the element you want to work with.
 2. Use its text content, child elements, and attributes.

When do we use Caching DOM Queries:
A: When we need to work with an element more than once. To store the result of the query we need to use **Variable**, but inside the variable is not the actual value but it is the *LOCATION* of the element in the DOM tree.

**NodeList:** Is a collection of nodes where the DOM query may return it when it wants to access it.
 **VIP** when accessing elements in node list is similar to the array; where it starts at index 0.

 There are two types of node lists:
  1. Live NodeList: When we update the script the node list will be updated as well.
  2. Static NodeList: When we update the script the node list might not be updated the changes made to the script.

What are the methods that are repnsible for selecting individual elements? 
A: We can use both getElementById() or querySelector().

Which one of these methods are desired more?
A: **getElementById()** because it is the quickest and more efficient way to access an element, because it is impossible to see two elements with the same ID. 
Where the **querySelector()** is still new to the DOM and it is not supported by older browsers.

Two ways for selecting an element an element form node list:
 1. Item() method: which will return an individual node from the Node list.  
 2. Array syntax: Where we can access the elements the same way we use to access the normal array.

 Selecting elements using class attributes:
 We use getElementbyClassName() where this method allows us to select elements whose class attribute contains specific value. 

Selecting elements using Tag Name:
getElementsByTagName () method allows us to select elements using their tag name.

Selecting Elements Using CSS Selectors:
querySelector() returns the first element node that matches the CSS-style selector. 

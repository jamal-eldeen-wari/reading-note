# Introductory to HTML, CSS and Javascript:
### Headings: 
It starts with h1 all the way to h6. HTML is known to have 6 level of heading where h1 is the largest heading and h6 is smallest heading.

### Paragraphs: 
HTML provides a way to create a paragraph by using p element once the browser sees this tag (which is the p tag i mean) by default the browser will show each paragraph in new line if we have multiple p tags.

### b tag: 
Any word inside the b tag will be **BOLD**.
### i tag: 
Any word inside the i tag will be **Italic**.
### sup tag: 
Is used to contain characters that should be superscript such as dates and mathmatical concepts.
### sub tag: 
it is commonly used for chemical formulas, it is used to contain any character that should be subscript.
### White Spacing: 
In HTML if there is two or more white spaces between words it will default make one space this is known as **white space collapsing**. 
### Break tag: 
When the browser sees a breaking tag it will automatically show each paragraph or heading in a new line.
### Horizontal tag: 
It is a way to create some seperation between themes (It is like creating a line between two paragraphs).
### Empty tag: 
Elements that do not have any words between the opening and closing tag.
### Strong tag: 
When we have a content that has a strong importance the word contained in this element might be said with strong emphasis.
### em tag: 
Indicates the emphasis that subtly changes the meaning of a sentence. Browser will show the content of em tag in **italic**.
### Blockqoute tag: 
it is used for longer qoutes that take up the entire paragraph. In a blockqoute element we can use p element inside of it. 
### q tag: 
It is used for shorter qoutes that sit within a paragraph. THere are browsers that do not support it such as Internet Explorer.
### abbr tag: 
It is used for abbreviation or an acronym it uses a title attribute to specify full term.
In HTML 4 there was an acronym tag specific for acronym it also sees the title to spell out the full form of acronym. Just like abbr tag in HTML 5.
### cite tag:
It is used for citation when you want to reference a piece of work we use cite attribute to indicate where the citation is. Once the browser sees this tag it will make its content as **italic**.
### dfn tag: 
It stands for definition it is used when you use a new terminology in a document. Some browsers change the content of the element dfn to **ITALIC**, where Safari and Google Chrome does not change its appearence.
### address tag: 
It is used to contain the content details for the author of the page, we can contain physical address.
### ins and del tags: 
ins standsfor insert where del standsfor delete. It works by showing the content that has been inserted to the document. Where as del tag shows what content has been removed from the document.
### s tag: 
It is used to indicate if something is not accurate or relevent. It is similar to the u tag used in HTML older versions.


## CSS:
It is a way of styling your HTML code to make it look very nice give it some life for our web page. In CSS we take the elements of HTML without the angled brackets hese elements are known as **Selector**. We can change the style of these elements which is known as **Declaration** for instance:
h1{
    color: red;
}
**h1 is Selector and the color:red is Declaration**.

**Important to note that the Declaration part is also divided into *Property* and *value***

### There are three ways to insert CSS to our HTML Code:
 1. External CSS: It is done by using seperate file that is usually called **style.css**. To use this style.css file in your code you need to use link tag to link our CSS file to HTML file, this link tag consists of two important attributes that are needed for the link:
  * href: file name with the path
  * rel: it specifies the relationship between HTML page and file that is linked.

 2. Internal CSS: There is no need to create CSS file. It is done by using style tag which is located at the head tag. Some people use the type attribute if there is number of CSS files.

 3. Inline Style: In the opening tag of that element you can add style and change the way that elemnet looks.


### CSS Selectors:
1. Universal Selector: Applies to all the elements in the document (*).
2. Type Selector: Matches the elements names that they are seperated with coma example(h1, h2, h3).
3. Class Selector: Any element with this class name will change it is appearance. used for more than one element (.).
4. ID Selector: Used for only one element it is unique for it (#).
5. Child Selector: Element that is a direct child of another (ul>li).

## Javascript Basic Instructions:
Variable declaration it is always starts with a **var** keyword and then you will need to give that variable a name and that name must be meaningful name for instance:
*var number;*

**Important to note** is that js knows that the var keyword is used to create a variable in js interpretor.

**Important to note** In case the var name is more than one word we cannot put spaces as we normal do in english class but we use the **camel case**. Camel Case concept is to keep the first letter of the word capital and the rest small letters.

Once the variable is declared we need to assign them to value and it happens by using **var name equals to the given value** example:
*number = 20;*.

### DATATYPES in js:
1. Numbers: It can take all numbers in the world either negative or positive.
2. String: Series of letters combined inside either double qoute or single qoute.
3. Boolean: It takes either true or false.

### Decision Making: 
When it comes to decision making alot of programmers like to use flowchart to help the plan.
flowchart is a graphical representation used by programmers as a planning tool to solve problem, it consists of symbols that are connected together to help them indicate the flow of info and processing.
Decision Making relies too much on comparison operators and logical operators (Are Binary).

#### Comparison Operators: 
* == : is equal to
* !=: is not equal to.
* ===: Strict equal to (Compares the value and the type).
* !==: Strict Not equal to (Compares the value and the type).
* Greater than.
* Less than 
* Greater than or equal.
* Less than or equal.

#### Logical Operators:
| Operand1     | Operand2   |     AND     |     OR      |NOT Operand1|
| ----------- | ----------- | ----------- | ----------- |----------- |
|     T       |      T      |       T     |       T     |      F     |
|     F       |      T      |       F     |       T     |      T     |
|     T       |      F      |       F     |       T     |      F     |
|     F       |      F      |       F     |       F     |      T     |

## IF Statement: 
It Uses the keyword IF to check the condition if the condition evaluates true then continue inside the IF body but IF it is false then exit the IF or go to else part.

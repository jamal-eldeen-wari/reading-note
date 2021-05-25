# HTML:
## Links:
In order to write links in HTML we use a tag (Anchor tag), where the user can click anything between the opening and closing tag you specify which page you want to link using href attribute.

**Important to note** that the text between the opening and closing tag is known as **Link Text**, where this link text will be shown in your webpage as a clickable link. Clear link text will help the visitors to find what they want easily.

So the link that you give your href will be the full web address for that particular site which is known as **Absolute URL**. URL Stands for *Uniform Resource Locator*.

When we want to link to other pages within the same site you do not need to specify the domain name in the URL we can use shorthand known as **Relative URL**.

**Relative URL**: Is used when we want to link other pages within the same site. It is also described as shorthand version of absolute URL because you do not need to specify the domain name.

To link an email in HTML we use MAILTO, where MAIL TO is not a tag we will still use a tag for it but we include it inside href attribute followed with Mail To: Email.

**VIP** When we open a link that uses MAIL TO it will take a user to new message and address it to the person specified in the link.

**Target**: It is an attribute used to open a new tab in your browser the value for it must be :_blank. It is used by authors who provides a link in his website.

**VIP** We should avoid opening links in a new window but if we do we must consider good practice to inform users that the link will open a new window before they click on it.

# CSS:
## Layout In CSS:
CSS treats every HTML element as if it is a box of its own this box can be either:
1. Block-Level Box.
2. Inline-Level Box.

As we mention before in our previous reads that block level element starts on a new line and inline element keeps them on the same side.
**Examples for elements in Block level**: 
(h1-h6, p, ul and li).

**Examples for elements in inline level**:
(img, b and i).

**Containing Element :** 
It occurs when a block level element sits inside another block level element then the outer box is known as **Containing** or **Parent element**.

**Positioning Scheme**:
CSS uses the positioning scheme to allow us to control the layout of a page:
 1. Normal Flow: Allows every element to appear in a new line (Block) causing each item to appear lower down the page than the previous one.

 2. Relative Positioning: It will move the element from one position where it would be in a normal flow shiffting it either to the top, bottom, right or left.

 3. Absolute Positioning: It is by positioning the elements in the relation to its containing element where it takes out normal flow. Meaning it does not affect position of surronding element.

**BOX OFFSET:**
It is used to indicate where the box should be positioning, where the box offset tells the browser how far from the top, bottom, left or right it should be placed.

**Fixed Positioning:** This is a form of absolute positioning that positions the element in relation to the browser window,as opposed to the containing element. Elements with fixed positioning do not move when the user scrolls up or down the page. Also they do not affect the position of surrounding elements.

**Floating Element:** allows us to take that element out of normal flow and position it to the far left or right of a containing box.

When we move any element from a normal flow it can cause box overlapping which may affect the **Z-index**. It is a property that allows us to control which box appears on top.

## Screen Sizes:
Most important factor when creating a website is that you need to consider the screen size of the visiting devices where they can very. Every device has its own resolution some devices has high resolution and others low. Resolution Means the number of dots a screen can show per inch.

**VIP** OS Allows us to adjust the screen resolution on our devices.

Because of the screen resolution variation designers often try to create pages around 960-1000 pixels wide.

## Fixed Layout:
### Advantages:
1. Pixel values are accurate at controlling size and positioning of elements.
2. The designer has far greater control over the appearance and position of items on the page than with liquid layouts.
3. The size of an image will always remain the same relative to the rest of the page.

### Disadvantages:
1. You can end up with big gaps around the edge of a page.
2. If the user's screen is a much higher resolution than the designer's screen, the page can look smaller and text can be harder to read.
3. The page will often take up more vertical space than a liquid layout with the same content.

## Liquid layout :
### Advantages:
1. Pages expand to fill the entire browser window so there are no spaces around the page on a large screen.
2. If the user has a small window, the page can contract to fit it without the user having to scroll to the side.
3. The design is tolerant of users setting font sizes larger than the designer intended.

### Disadvantages:
1. if you do not control the width of sections of the page then the design can look very different than you intended, with unexpected gaps around certain elements or items squashed together.
2. If the user has a wide window, lines of text can become very long, which makes them harder to read.
3. If the user has a very narrow window, words may be squashed and you can end up with few words on each line.

# JAVASCRIPT:
## Functions: 
Is a very important topic in js. Functions in coding is like tiding your room put every thing where it belongs makes the code look better more readable.

### Function Declaration:
It starts with function keyword and folows it the function name where the name must be useful then we include paranthisis inside the paranthisis can be empty or we can have an input ot number of inputs.
**Syntax**
function getData(input)
{
    Some code
    return;

}

TO Invoke or call a function we call it from its name for instance:
getData();

# Pair Programming:
It is a way where two programmers can work together to Iterative loops, Code reviews, Fast feedback and Error checking and linting. It is one of the tactics that code fellows uses to foster a collaborative environment while developing key industry skills. Similar to rally races where you will find a driver and navigator same thing here in programming, The Driver is the programmer who is typing and the only one whose hands are on the keyboard. Handling the “mechanics” of coding, the Driver manages the text editor, switching files, version control, and—of course writing—code. The Navigator uses their words to guide the Driver but does not provide any direct input to the computer. The Navigator thinks about the big picture, what comes next, how an algorithm might be converted in to code, while scanning for typos or bugs. The Navigator might also utilize their computer as a second screen to look up solutions and documentation, but should not be writing any code.

Benefit of using pair programming:
1. Greater efficiency
2. Engaged collaboration
3. Learning from fellow students
4. Social skills
5. Job interview readiness
6. Work environment readiness


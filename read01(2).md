# Introductory to HTML and JS:
This book has been written to help those who want to learn how to build websites from scratch and for anyone who want more control over the apperence of their page.

## How the web works:
1. When visiting a website, that website will be on a webserver and that webserver  can be anywhere around the world in order to find that webserver that is hosting our targeted website, our browser will have to connect to something called **Domain Name Server (DNS)**. 

2. DNS will tell your browser where to find the webserver that hosts that website.

3. Then the webserver returns the requested page to your web browser.

**Domain Name Server(DNS)**: It is a network of servers it acts as a phone book it they tell your computer
the IP address associated with the requested domain name. And every device connected to the internet has a unique identification number that is called IP.

**Internet Protocol**: Is a 12 digit number that is seperated by periods it act as a phone number for that computer.

**WebServer**: Is a computer that is constantly connected to the web. Main job for the webserver is to send web pages to users.

## HTML:
*It is used to describe the structure of the page.* Main HTML elements:
* <html> element: Anything between the opening and the closing tag of the html is an HTML code.
* <body> element: Anything between the opening and closing tag should be shown inside the main browser window.

* <h1>-<h6> elements: Main Heading for html.
* <p> element: paragraph.

**Attributes in HTML**: They appear in the opening tag and are made up of two parts name and value seperated by equal sign.

### HTML Versions:
Over the years there has been number of HTML versions and every version of HTML is an improvement over the old version provides more featrues. Main problem here is how the browser will know what version to use? in this case we use "DOCTYPE".

Benefits of using DOCTYPE: 
* It tells the browser what version of html will it use.
* It helps to render the page correctly.

**HTML Versions**:

1. XML.

2. XHTML.

3. HTML 4.

4. HTML 5.

### Comment In HTML:
To add a comment in html we use "<!-- -->" known as inline comment. Comments are very useful for programmers, it helps them to know what does this part of code does or can be some notes to help colleagues to understand the code.

### ID in HTML:
It is used to uniquely identify element from other elements the value of the id should start with **letter or underscore** NOT a number or any special character.

**important to note** that we cannot have two or more elements the same id, the id must be unique for that element.

**Benefit for having an ID**
is that in CSS you can have a different style for that element in case that element is VIP and we want to make it unique.

ID attribute is known as *global attribute*

### Class Attribute:
Number of elements have the same class name it is like a family where the members of that family can have that name. 

**Important to note** Class attribute can share its value with other element unlike the ID.

Using either Class or ID attributes does not effect the presentation of the element but it changes their appereance if used in CSS.

### Block Elements: 
They will always appear to start on a new line in browser window some of the Block Elements: (<h1>, <ul>, <ol>, <li> and <p>).
### inline Element:
Elements that continue on the same line in browser window. Some of Inline element (<a> and <img>).

### Grouping text and elements in a block: 
The only element that is responsible for grouping is <div> element. It groups a set of elements together in one block-level box. <div> element is similar to block element because the contents of <div> elements will start in a new line.

### Grouping text and elemnts inline: 
The only elemnts that is responsible for grouping in line is the <span> element. There are two ways to use it:

1. Contain a section of text where there is no other suitable element to diffrerentiate it from its surronding text.

2. Contain a number of inline element.

**Important to note** with the span element you will usually see that class or id being used with it.

### <iframe> element:
Little window that has been cut into your page it is mainly used to embed google maps in your website.

**iframe has number of attributes**:

1. width.

2. height.

3. src: used for URL.

4. Scrolling: This attribute is not supported with HTML5 it is goal is to make the little window scrollable or not.

5. Frameborder: Not supported in HTML 5 it indecates whether the frame has a border or not takes two values either 0 or 1.

6. Seamless: Supported in HTML 5 it can be applied to an iframe where scroll bars are not desired. Older browsers does not support it.

### <Meta> Element: 
It lives inside the <head> tag, contains information about that webpage its not visible to user but it fullfills number of purposes such as:

1. Telling search engine about the page and who created it.

2. Meta element is an empty element that does not have a closing tag.

**Common Attributes for Meta**:

1. Name attribute

2. Content attribute.

### <header> and <footer> Elements:
Header appears top of the page where footer appears at the bottom of the page.

### <nav>: 
It is used to contain the major navigational block on the site such as primary site navigation.

### <artical>:
It acts as a container for any section of a page that could standalone and potentially be syndicated. We can have multiple articals elements in a page and we can have nested articals.

### <aside>:
Has two purposes:

1. when aside element is used inside of an artical elementit should contain information that is related to the artical.

2. When aside element is being used outside of artical element it acts like a container for the content for the related page.

### <section> :
It groups together the related content and each section would have it is own heading.
in case of any long artical in our page we can split it up by using section.

Section Element should not be used as wrapper for the entire page the best element for the wrapping is <div>.

### <hgroup>:
It is used to group a set of one or more <h1> through <h6> so that they are treated as one single heading.

### <Figure>: 
It can be used to contain any content that is referenced from the main flow of the artical.

Figure elements can be used for: 
* images.
* Video.
* Graphs.
* Diagrams.
* Code Samples.
* Text that supports main body of the artical.

### <a>:
Is used to link around block-level element that contains child element it allows us to make the entire block a link.
 
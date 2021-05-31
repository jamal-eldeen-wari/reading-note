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

## Position Attribute:
It is used to change the layout of your website, with the position attribute we can use some values such as:
 1. Static value: it is used in normal flow, each block-level element sits on top of the next one.This is the default way where browsers treat HTML elements. Writing the attribute in CSS: position:static.
 2. Relative Value: it moves an element in relation to where it would have been in normal flow.
 3. Absolute Value: By using the absolute value the box is taken out  of normal flow and no longer affects the 
 position of other elements on the page.
 4. Fixed Value: is a type of absolute positioning that requires the position property to be fixed

## Overlapping Elements: 
It can occur when using relative, absolute or fixed positioning, it happens by making the box overlap on other HTML elements to overcome this issue we can use **Z-index** property where it allows us to control which elements sits on top.The higher the value of the z-index the closer that element is to the front.

## Floating Elements: 
It allows us to take an element in normal flow and place it as far to the left or right of containing element as possible.Anything that sits inside the containing element will flow around the element that its floated.
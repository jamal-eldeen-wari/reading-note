# HTML & CSS Introductory:

## lists in HTML:
Two types of lists in HTML:
1. Unordered List: It creates a list with dots count (UL tag).
2. Ordered List: It creates a list with number count (OL tag).
**These two lists use a tag called *list items*. Where the li tag is used as much as you want elements in your browser.**

Other types of list that HTML support: 
* dl tag: It is used for series of terms and definitions. Inside dl you will see pairs of elements:
 1. dt tag: It is used to contain the term being defined.
 2. dd tag: It is used to contain the definition itself.

**Important TO Note** in list we can have *Nested lists*, it works by adding second list inside of the li tag. Usually the browser view the nested list indented further than the parent list (For Ordered). But for Unordered the browser usually change the style of the bullet point too.

## Boxes:
The most popular way of sizing boxes are to use pixels, percentage or ems. But popular one of them is **Pixel** because it allows the designers to accuratlly control their size. **Percentage** when we use % the size of the box is relative to the size of the browser window. **ems** when we use ems the size of the box is based on the size of the text within it.

**Important to note** is that both the % and ems are started to be used by the developer because these two measurments showed their flexability accross devices which have different sized screens.

To ensure that the content of pages are legible we use :
Min width property: Specifies the smallest size box can be displayed when the browser window is **narrow**.

max height Property: Indicates the maximum width of a box can stretch to when browser window is width 

**Overflowing property**: tells the browser what to do if the content contained within the box is larger than the box itself.

There are two value for overflow: 
1. Hidden: Simply hides any extra context that does not fit the box.
2. scroll: Adds scrollbar to the box so that users can scroll to see missing parts.

**important to note** We can come to conclusion is that overflow property is very important because some browsers allow users to adjust the size of the text to appear as large or small as they want.

Three important properties for every box: 
1. Border: It seperate the edge of the one box from another.
2. Margin: It sits outside of the edge of the border its used to create gap between the borders of the two adjacent boxes.
3. Padding: Is the space between the border of the box and any content contained within it.

 Adding padding can increase the readability of it is contents.

 **Border** has some properties:
 1. Border width: Is used to control the width of the border. Values can be either in pixels or (thin, medium and thick). We cannot use % in the width border.
 2. Border Style: it takes the following values:
   * Solid 
   * Dotted
   * Dashed
   * Double
   * Groove
   * Ridge
   * Inset
   * Outset
   * Hidden

3. Border Color: It is possible to individually control the colors of the border on different size. which is one of the flexibility with border.

**Important to note** You can specify all of the previous properties in one property by using border property and putting the value with space between each type.

**Padding**: As we mentioned before that padding allows us to specify how much space should be between the element and the border.
The value for padding is often used in pixels but we can also use % and ems.

**Important to note** if we add width for a box and then we add padding that padding is added to the width of the box.

**Margin**: Controlls the gap between boxes and its value is commonly used in pixels and we can also still use % and ems.
If one box sits on top of another margins are collapsed which means the larger of the two will be used and the smaller will be discard.

**Important to note** that the value of the margin is not inherited by child element in the same way font-family and color value.

In order to center any box in the middle we need to set the left-margin and the right margin to **auto**

**Display Property**: It allows us to turn an inline element into block level element or vice versa and can be used to hide an element from the page.

Display property value: 
 . Inline Element: It makes the block element act as Inline element.
 2. Block Element: It makes Inline Element act as block Element.
 3. Inline-Block: It causes the Block-level element to flow like Inline Element.
 4. none: Hids the element from the page.

**Box Shadow Property**: It allows us to drop a shadow around a box, it works just like text shadow property.









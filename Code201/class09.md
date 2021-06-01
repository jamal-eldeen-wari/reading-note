# Forms:
It is best known on the web it can be used when registering to website or shopping online.
## Form Control:
 1. Adding Text: Used for single line of text for instance in name, email and address.
 2. Making Choice: There are three types of it:
   1. Radio Buttons: It only allows you to select one of the options such as gender
   2. Checkboxes: it allows the user to check or uncheck one of the options or more.
   3. Drop-down boxes: Allows the user to pick number of options from a list.

## Form Structure in HTML:
To form a structure in HTML we use the following Tags:
1. form tag: This element should always carry the action attribute and will usually have a method and id attribute too some of the attributes:
  * action: Every form requires an action attribute its value is the URL for the page on the server that will receive the information in the form when it is submitted.
  * method: Forms can be sent using one of two methods: get or post.With the get method, the values 
    from the form are added to the end of the URL specified in the action attribute.
    FOR THE GET:
     1. short forms
     2. when you are just retrieving data from the web server.
    FOR THE POST:
     1. allows users to upload a file
     2. is very long
     3. contains sensitive data
     4. adds information to, or deletes information from, a database.
    
    **Important to note** if the method attribute is not used, the form data will be sent using the get method.

  * ID: the value is used to identify the form distinctly from other elements on the page.

## Text Input: 
it is used to create several different form controls. The value of the typeattribute determines what kind of input they will be creating. It has a number of attributes:
 1. type: When the type attribute has a value of text, it creates a single-line text input.
 2. name: When users enter information into a form, the server needs to know which form control each piece of data was entered into.
 3. size: It was used in older forms to indicate the width of the text input 
  **VIP** This attribute should not be used in new forms
 4. Max Length: It can be used to limit the number of characters a user may enter into the text field. Its value is the number of characters they may enter.

## Password Input: 
  Some of the important attributes used with password input:
  1. type:it creates a text box that acts just like a single-line text input, except the characters are blocked out. They are hidden in this way so that if someone is looking over the user's shoulder, they cannot see sensitive data such as passwords.
  2. name: The name attribute indicates the name of the password input, which is sent to the server with the password the user enters.
  3. size or max length: It can also carry the size and maxlength attributes like the the single-line text input.

## Text Area: 
its used to create a mutli-line text input. Unlike other input elements this is not an empty element. It should therefore have an opening and a closing tag.

## Radio Button: 
Radio buttons allow users to pick just one of a number of options. It uses some attributes:
 1. name: e is sent to the server with the value of the option the user selects. When a question provides users with options for answers in the form of radio buttons, the value of the name attribute should be the same for all of the radio buttons used to answer that question.
 2. value: it indicates the value that is sent to the server for the selected option. The value of each of the buttons in a group should be different.
 3. checked: it can be used to indicate which value should be selected when the page loads.   

**VIP** Once the radio button is selected it cannot be removed at all you can still click on the rest.

## Check Box: 
Checkboxes allow users to select one or more options in answer to a question. It has some attributes:
 1. name: The name attribute is sent to the server with the value of the optionthe user selects. 
 2. value: The value attribute indicates the value sent to the server if this checkbox is checked.
 3. Checked: The checked attribute indicates that this box should be checked when the page loads. If used, its value should be checked.  

## Drop Down List: 
allows users to select one option from a drop down list. it uses the select tag to create a drop down list box. It 
contains two or more options elements.

# CSS:
## Bullet point style:
The list-style-type property allows you to control the shape or style of a bullet point (also 
known as a **marker**). It can also be used with ul, ol and li tags.

## Image for bullets:
You can specify an image to act as a bullet point using the list-style-image property.

## Positioning the marker:
Lists are indented into the page by default and the list-style-position property indicates whether the marker should appear on the inside or the outside of the box containing the main points. Where the list-style-position has two values: 
 1. outside: The marker sits to the left of the block of text.
 2. inside: The marker sits inside the box of text.

## List Short hand:
As with several of the other CSS properties, there is a property that acts as a shorthand for list styles. It is called list-style, and it allows you to express the markers' style, image and position properties in any order.  

## Border on empty cell:
If you have empty cells in your table, then you can use the empty-cells property to specify whether or not their 
borders should be shown. it has three values: 
 1. show: This shows the borders of any empty cells.
 2. hide: This hides the borders of any empty cells
 3. inherit: If you have one table nested inside another, the inheritvalue instructs the table cells to obey the rules of the containing table.

 ## Styling text inputs: 
 Most commonly used attributes in CSS:
 1. font-size: sets the size of the text entered by the user.
 2. color and background color.
 3. border: adds a border around the edge of the input box, andborder-radius can be used to create rounded corners.
 4. focus: is pseudo-class used to change the background color of the text input when it is being used.
 5. background image: adds a background image to the box. 
 
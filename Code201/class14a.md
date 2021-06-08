# Transform in CSS:
Since CSS3 came out it provided new ways to position and alter elements. Because of transfom in CSS we can now have some general layout techniques can be revisited with alternative ways to size, position, and change elements. 

Transform Property has **two different settings:**
 1. two-dimensional.
 2. three-dimensional.

 **Transform Syntax:** 
 The actual syntax for the transform property is quite simple, including the transform property followed by the value. As we can see taht the transform property includes multiple vendor prefixes to gain the best support across all browsers. The un-prefixed declaration comes last to overwrite the prefixed versions it does that because not all browsers support transform property.

 ## 2D Transfom:
 Two-dimensional transforms work on the x and y axes, known as horizontal and vertical axes.
 **2D has some values that it supports such as:**
  1. rotate: provides the ability to rotate an element from **0 to 360** degrees. Using a *positive* value will **rotate an element clockwise**, and using a *negative* value will **rotate the element counterclockwise**. The default point of rotation is the center of the element, 50% 50%, both horizontally and vertically.

  2. Scale: Using the scale value within the transform property allows you to change the appeared size of an element. The default scale value is 1, therefore any value between .99 and .01 makes an element appear smaller while any value greater than or equal to 1.01 makes an element appear larger.
  It is possible to scale only the height or width of an element using the **scaleX and scaleY values**. The scaleX value will scale the width of an element while the scaleY value will scale the height of an element. o scale both the height and width of an element but at different sizes, the x and y axis values may be set simultaneously. To do so, use the scale transform declaring the x axis value first, followed by a comma, and then the y axis value.

  3. Translate: The translate value works a bit like that of **relative positioning, pushing and pulling an element** in different directions without interrupting the normal flow of the document. Using the translateX value will change the position of an element on the horizontal axis while using the translateY value will change the position of an element on the vertical axis.
  **Measurment for translate can be either pixels or percentages are common.**
  
  4. Skew: is used to distort elements on the horizontal axis, vertical axis, or both. The syntax is very similar to that of the scale and translate values. Using the skewX value distorts an element on the horizontal axis while the skewY value distorts an element on the vertical axis. To distort an element on both axes the skew value is used, declaring the x axis value first, followed by a comma, and then the y axis value.

  ## Combining Transforms:
  It is common for multiple transforms to be used at once, rotating and scaling the size of an element at the same time. To make it work we need to combine them together but not making multiple transfom declarations will not work.

  ## Transform Origin:
  the default transform origin is the dead center of an element, both 50% horizontally and 50% vertically. To change this default origin position the transform-origin property may be used. Where it can accept one or two values. When only one value is specified, that value is used for both the horizontal and vertical axes. If two values are specified, the first is used for the horizontal axis and the second is used for the vertical axis.


 ## 3D Transfom:
 Three-dimensional transforms work on both the x and y axes, as well as the z axis. These three-dimensional transforms help define not only the length and width of an element, but also the depth.
 **3D has some values that it supports such as:**
  1. Rotate: Similar to 2D but the only difference is here we are going to use z axis.
  2. Scale: Similar to 2D but the only difference is here we are going to use z axis.
  3. Translate: Similar to 2D but the only difference is here we are going to use z axis.
  4. Skew: Skew is the one two-dimensional transform that cannot be transformed on a three-dimensional scale. Elements may be skewed on the x and y axis, then transformed three-dimensionally as wished, but they cannot be skewed on the z axis.

 ## Prespective:
 In order for three-dimensional transforms to work the elements need a perspective from which to transform. The perspective for each element can be thought of as a vanishing point, similar to that which can be seen in three-dimensional drawings.

 Prespective can be set in two different ways:
  1. One way includes using the perspective value within the transform property on individual elements.
  2. Other way includes using the perspective property on the parent element residing over child elements being transformed.

Benefit of using prespective that it works great for transforming one element from a single, unique perspective. When you want to transform a group of elements all with the same perspective, or vanishing point, apply the perspective property to their parent element.

## Transform Style:
On occasion three-dimensional transforms will be applied on an element that is nested within a parent element which is also being transformed. In this event, the nested, transformed elements will not appear in their own three-dimensional space. To allow nested elements to transform in their own three-dimensional plane use the transform-style property with the preserve-3d value.

# Transition & Animations:
It emerges in the CSS3 where it gave us the ability to write behaviors for transitions and animations. Front end developers have been asking for the ability to design these interactions within HTML and CSS, without the use of JavaScript or Flash, for years. Now their wish has come true.

With CSS3 transitions we have the potential to alter the appearance and behavior of an element whenever a state change occurs, such as when it is hovered over, focused on, active, or targeted.

Animations within CSS3 allow the appearance and behavior of an element to be altered in multiple keyframes. Transitions provide a change from one state to another, while animations can set multiple points of transition upon different keyframes.

## Transitions in CSS:
Where an element must have a change in state, and different styles must be identified for each state. The easiest way for determining styles for different states is by using the pseudo-classes such as :hover, :focus, :active, and :target.

Transitions have four properties:
 1. transition-property: determines exactly what properties will be altered in conjunction with the other transitional properties. By default, all of the properties within an element’s different states will be altered upon change. However, only the properties identified within the transition-property value will be affected by any transitions.

 2. transition-duration:he value of this property can be set using general timing values, including seconds (s) and milliseconds (ms). These timing values may also come in fractional measurements.

 3. transition-timing-function: is used to set the speed in which a transition will move. Knowing the duration from the transition-duration property a transition can have multiple speeds within a single duration. A few of the more popular keyword values for the transition-timing-function property include linear, ease-in, ease-out, and ease-in-out.

 4. transition-delay: On top of declaring the transition property, duration, and timing function, you can also set a delay with the transition-delay property. The delay sets a time value, seconds or milliseconds, that determines how long a transition should be stalled before executing.

 ## Shorthand Transition:
 sing the transition value alone, you can set every transition value in the order of transition-property, transition-duration, transition-timing-function, and lastly transition-delay. Do not use commas with these values unless you are identifying numerous transitions.

 # Animations in CSS:
 It uses feyframes To set multiple points at which an element should undergo a transition, use the @keyframes rule. The @keyframes rule includes the animation name, any animation breakpoints, and the properties intended to be animated.

 Animation Name:
 Once the keyframes for an animation have been declared they need to be assigned to an element. To do so, the animation-name property is used with the animation name, identified from the keyframes rule, as the property value. The animation-name declaration is applied to the element in which the animation is to be applied to. 

 Animation Duration, Timing Function, & Delay:
 animations behave similarly to transitions. They include a duration, timing function, and delay if desired. To start, animations need a duration declared using the animation-duration property. As with transitions, the duration may be set in seconds or milliseconds.  


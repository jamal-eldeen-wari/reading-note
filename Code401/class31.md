# Espresso:
It is used to write concise, beautiful, and reliable Android UI tests.

The core API is small, predictable, and easy to learn and yet remains open for customization. Espresso tests state expectations, interactions, and assertions clearly without the distraction of boilerplate content, custom infrastructure, or messy implementation details getting in the way.

## Some of espresso API Components:
1. Espresso: This is the starting point for all test cases. It starts the interactions with the app’s view. Each app’s view has two components.

2. ViewMatchers: Views are always in a **hierarchy** called the View Hierarchy. ViewMatchers are used when we want to navigate a view hierarchy.

3. ViewActions: These components define the action that has to be performed on any given View. Espresso allows testers to send more than one ViewAction as a collection to the Interaction method.

4. ViewAssertions: They are the components that check if the test has passed or failed.

## Some Important Functions In Espresso:
1. onView: Using this function, we can **narrow down to the desired view in the view hierarchy**.Once this method is invoked  Espresso waits to perform the corresponding UI action or assertion until the following synchronization conditions are met:

1. The message queue is empty. 
2. There are no instances of AsyncTask currently executing a task.
3. All developer-defined idling resources are idle.

It can be done by using the following functions inside onview:
 * withId().
 * withText().

2. check: It is used to check the behavior of the desired view, such as  visibility, focus, and more by using **matches** and **doesNotExist**.

3. perform: It is used to execute actions on a specific view. Some functions that can be used with it in espresso:
 1. click() method.
 2. typeText() Method.
 3. replaceText() Method.
 4. closeSoftKeyboard() Method Used in thursday demo.


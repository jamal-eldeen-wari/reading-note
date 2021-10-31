# Android Studio:

## Tasks and the back stack:
A task is a collection of activities that users interact with when trying to do something in your app. These activities are arranged in a stack—the back stack—in the order in which each activity is opened.

## Lifecycle of a task and its back stack
The device Home screen is the starting place for most tasks. When a user touches the icon for an app or shortcut in the app launcher (or on the Home screen), that app's task comes to the foreground. If no task exists for the app (the app has not been used recently), then a new task is created and the main activity for that app opens as the root activity in the stack.

When the current activity starts another, the new activity is pushed on the top of the stack and takes focus. The previous activity remains in the stack, but is stopped. When an activity stops, the system retains the current state of its user interface. When the user performs the back action, the current activity is popped from the top of the stack (the activity is destroyed) and the previous activity resumes (the previous state of its UI is restored). Activities in the stack are never rearranged, only pushed and popped from the stack—pushed onto the stack when started by the current activity and popped off when the user leaves it using the Back button or gesture. As such, the back stack operates as a last in, first out object structure. 

## Background and foreground tasks:
A task is a cohesive unit that can move to the background when a user begins a new task or goes to the Home screen. While in the background, all the activities in the task are stopped, but the back stack for the task remains intact—the task has simply lost focus while another task takes place.

## Multiple activity instances:
Because the activities in the back stack are never rearranged, if your app allows users to start a particular activity from more than one activity, a new instance of that activity is created and pushed onto the stack (rather than bringing any previous instance of the activity to the top).



## Save Key Value Data:
You can create a new shared preference file or access an existing one by calling one of these methods:

1. getSharedPreferences() — Use this if you need multiple shared preference files identified by name, which you specify with the first parameter. You can call this from any Context in your app.

2. getPreferences() — Use this from an Activity if you need to use only one shared preference file for the activity. Because this retrieves a default shared preference file that belongs to the activity, you don't need to supply a name.

To **write to a shared preferences file**, create a SharedPreferences.Editor by calling edit() on your SharedPreferences.

**Read from shared preferences** to retrieve values from a shared preferences file, call methods such as getInt() and getString(), providing the key for the value you want, and optionally a default value to return if the key isn't present.

When naming your shared preference files, you should use a name that's uniquely identifiable to your app. An easy way to do this is prefix the file name with your application ID.

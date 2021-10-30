# Android Studio:
Android app can be written in Java, Kotlin and C++.

## What is Android SDK ??
Are tools compile your code along with any data and resource files into an APK or an Android App Bundle.

## What is Android Package ??
s an archive file with an .apk suffix, contains the contents of an Android app that are required at runtime and it is the file that Android-powered devices use to install the app.

An **Android App Bundle**, which is an archive file with an **.aab suffix**, contains the contents of an Android app project including some additional metadata that is not required at runtime. An **AAB** is a publishing format and is not installable on Android devices, it defers APK generation and signing to a later stage. When distributing your app through Google Play for example, Google Play's servers generate optimized APKs that contain only the resources and code that are required by a particular device that is requesting installation of the app.

**Important to note** that Android operating system is a multi-user Linux system in which each app is a different user.

The Android system **implements the principle of least privilege**. That is, each app, by default, has access only to the components that it requires to do its work and no more. This creates a very secure environment in which an app cannot access parts of the system for which it is not given permission.

## App Component: Android system can start an app component
are the essential building blocks of an Android app. Each component is an entry point through which the system or a user can enter your app. Some components depend on others.

There are four different types of app components:

1. Activities: is the entry point for interacting with the user. It represents a single screen with a user interface. It is done by implementing an activity as a subclass of the Activity class. 

2. Services: is a general-purpose entry point for keeping an app running in the background for all kinds of reasons. It is a component that runs in the background to perform long-running operations or to perform work for remote processes. A service does not provide a user interface.

3. Broadcast receivers:is a component that enables the system to deliver events to the app outside of a regular user flow, allowing the app to respond to system-wide broadcast announcements. Because broadcast receivers are another well-defined entry into the app, the system can deliver broadcasts even to apps that aren't currently running. 

4. Content providers: A content provider manages a shared set of app data that you can store in the file system, in a SQLite database, on the web, or on any other persistent storage location that your app can access. 

## Activating components:
Three of the four component types—activities, services, and broadcast receivers—are activated by an asynchronous message called an **intent**. 
**Intents bind individual components to each other at runtime**. 

An intent is created with an Intent object, which defines a message to activate either a specific component (explicit intent) or a specific type of component (implicit intent).

## Manifest File:
Android system can start an app component, the system must know that the component exists by reading the app's manifest file.

List the thing the manifest does:
1. Identifies any user permissions the app requires, such as Internet access or read-access to the user's contacts.

2. Declares the minimum API Level required by the app, based on which APIs the app uses.

3. Declares hardware and software features used or required by the app, such as a camera, bluetooth services, or a multitouch screen.

4. Declares API libraries the app needs to be linked against (other than the Android framework APIs), such as the Google Maps library.


**How can we declare components ??**
The primary task of the manifest is to inform the system about the app's components.
Activities, services, and content providers that you include in your source but do not declare in the manifest are not visible to the system and, consequently, can never run. However, broadcast receivers can be either declared in the manifest or created dynamically in code as BroadcastReceiver objects and registered with the system by calling registerReceiver().


## App Resources:
An Android app is composed of more than just code—it requires resources that are separate from the source code, such as images, audio files, and anything relating to the visual presentation of the app.

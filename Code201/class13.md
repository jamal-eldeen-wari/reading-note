# Local Storage:
What is persistant local storage??
A: Well it was used by the native client application where it had some advantages over the web applications. As the native application typically provides an abstraction layer for storing and rerieving  application-specific data like preferences or runtime state. These values may be stored in the registry, INI files(Initialization Files), XML files (extensible markup language), or some other place according to platform convention. If your native client application needs local storage beyond key/value pairs, you can embed your own database, invent your own file format, or any number of other solutions

**Important to note that the web did not have the ability to store data unlike the native application** But cookies where invented early in the webs history that can be used to persistent local storage of small amounts of data but they had three downsides:
 1. Cookies are included with every HTTP request, thereby slowing down your web application by needlessly transmitting the same data over and over.
 2. Cookies are included with every HTTP request, thereby sending data unencrypted over the internet.
 3. Cookies are limited to about 4 KB of data — enough to slow down your application (see above), but not enough to be terribly useful.

The specs that are really desiered are:
 1. a lot of storage space on the client that persists beyond a page refresh and isn’t transmitted to the server.

## HTML5 Storage:
It can also be refered to as Web Storage which was at one time part of the HTML5 specification properbut was split out into its own specification for uninteresting political reasons. Certain browser vendors also refer to it as **Local Storage** or **DOM Storage.** The naming situation is made even more complicated.

So HTML5 Storage: it’s a way for web pages to store named **key/value** pairs locally, within the client web browser. Like cookies, this data persists even after you navigate away from the web site, close your browser tab,or exit your browser. Unlike cookies, this data is never transmitted to the remote web server.

Web Browsers that supported HTML5 Storage:
 1. IE (Internet Explorar)version 8.0+.
 2. Firefox 3.5+
 3. Safari 4.0+
 4. Chrome 4.0+
 5. Opera 10.5+
 6. Iphone 2.0+
 7. Android 2.0+

Before using html 5 we need to check whether our browser supports it or not and it is done by:



function supports_html5_storage() {

  try {

    return 'localStorage' in window && window['localStorage'] !== null;

  } 

  catch (e) {

    return false;

  }

}

OR we can use Modernizr to check if our browser supports HTML5 or not


if (Modernizr.localstorage) {


  // window.localStorage is available!


} 


else {


  // no native support for HTML5 storage :(


  // maybe try dojox.storage or a third-party solution


}


As we discussed earlier HTML5 Storage is based on named key/value pairs. You store data based on a named key, then you can retrieve that data with the same key. The named key is a string. The data can be any type supported by JavaScript, including strings, Booleans, integers, or floats. However, the data is actually stored as a string. If you are storing and retrieving anything other than strings, you will need to use functions like parseInt() or parseFloat() to coerce your retrieved data into the expected JavaScript datatype.

How can we keep tracking our storage:
By trapping the storage event. Is fired on the window object whenever setItem(), removeItem(), or clear() is called and actually changes something.For instance: if we set an item to its existing value or call clear() when there are no named keys, the storage event will not fire, because nothing actually changed in the storage area.
So the storage event is very important whenever this storage event is supported the localStorage object is supported, which includes Internet Explorer 8. IE 8 does not support the W3C standard addEventListener.
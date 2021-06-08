# LOCAL STORAGE

Persistent local storage is one of the areas where native **client applications** have held an advantage over **web applications**. For native applications, the operating system typically provides an abstraction layer for storing and retrieving **application-specific** data like preferences or runtime state. These values may be stored in the **registry, INI files, XML files**, or some other place according to platform convention. If your native client application needs local storage beyond key/value pairs, you can embed your own database, invent your own file format, or any number of other solutions.

Cookies  have three potentially dealbreaking downsides:

- Cookies are included with every HTTP request, thereby slowing down your web application by needlessly transmitting the same data over and over

- Cookies are included with every HTTP request, thereby sending data unencrypted over the internet (unless your entire web application is served over SSL)

- Cookies are limited to about 4 KB of data — enough to slow down your application (see above), but not enough to be terribly useful

## INTRODUCING HTML5 STORAGE

What I will refer to as “HTML5 Storage” is a specification named **Web Storage**, which was at one time part of the HTML5 specification proper, but was split out into its own specification for uninteresting political reasons. Certain browser vendors also refer to it as **“Local Storage”** or **“DOM Storage.”**

## HTML5 STORAGE SUPPORT

- ### `IE 8.0+`, `FIREFOX 3.5+`, `SAFARI 4.0+`, `CHROME 4.0+`, `OPERA 10.5+`, `IPHONE 2.0+`, `ANDROID 2.0+`

From your **JavaScript code**, you’ll access HTML5 Storage through the `localStorage` object on the **global window object**. Before you can use it, you should detect whether the **browser supports it**.

- ### check for HTML5 Storage

```js
function supports_html5_storage() {
  try {
    return 'localStorage' in window && window['localStorage'] !== null;
  } catch (e) {
    return false;
  }
}
```

Instead of writing this function yourself, you can use `Modernizr` to detect support for HTML5 Storage.

```js
if (Modernizr.localstorage) {
  // window.localStorage is available!
} else {
  // no native support for HTML5 storage :(
  // maybe try dojox.storage or a third-party solution
}
```

- ### USING HTML5 STORAGE

HTML5 Storage is based on named **key/value** pairs. You store data based on a named key, then you can retrieve that data with the same key. The named key is a string. The data can be any type supported by JavaScript, including `strings`,`Booleans`, `integers`, or `floats`. However, the data is actually stored as a `string`. If you are storing and retrieving anything other than strings, you will need to use functions like `parseInt()` or `parseFloat()` to coerce your retrieved data into the expected JavaScript datatype.

```js
interface Storage {
  getter any getItem(in DOMString key);
  setter creator void setItem(in DOMString key, in any data);
};
```

Calling `setItem()` with a named key that **already exists will silently overwrite the previous value**. Calling `getItem()` **with a non-existent key will return null rather than throw an exception**.

Like other JavaScript objects, you can treat the `localStorage` object as an **associative array**. Instead of using the `getItem()` and `setItem()` methods, you can simply use **square brackets**. For example, this snippet of code:

```js
var foo = localStorage.getItem("bar");
// ...
localStorage.setItem("bar", foo);
```

Could be rewritten to use square bracket syntax instead:

```js

var foo = localStorage["bar"];
// ...
localStorage["bar"] = foo;
```

There are also methods for removing the value for a given named key, and clearing the entire storage area (that is, deleting all the keys and values at once).

```js
interface Storage {
  deleter void removeItem(in DOMString key);
  void clear();
};
```

Calling `removeItem()` with a **non-existent key will do nothing**.

If you call `key()` with an index that is not **between 0–(length-1)**, the function will **return null**.

### TRACKING CHANGES TO THE HTML5 STORAGE AREA

If you want to keep track programmatically of when the storage area changes, you can **trap** the storage event. The storage event is fired on the **window object whenever** `setItem()`, `removeItem()`, or `clear()` is called and actually changes something. For example, if you set an item to its existing value or call `clear()` when there are no named keys, the storage event will not fire, because nothing actually changed in the storage area.

The storage event is supported everywhere the localStorage object is supported, which includes Internet Explorer 8. IE 8 does not support the W3C standard addEventListener (although that will finally be added in IE 9). Therefore, to hook the storage event, you’ll need to check which event mechanism the browser supports. 

```js
if (window.addEventListener) {
  window.addEventListener("storage", handle_storage, false);
} else {
  window.attachEvent("onstorage", handle_storage);
};
```

The handle_storage **callback** function will be called with a `StorageEvent` object, except in **Internet Explorer** where the event object is stored in `window.event`.

```js
function handle_storage(e) {
  if (!e) { e = window.event; }
}
```

- ### STORAGEEVENT OBJECT

| PROPERTY |  TYPE | DESCRIPTION |
|:-------- | :---- |:------------|
| key      | string| the named key that was added, removed, or modified|
| oldValue | any   | the previous value (now overwritten), or null if a new item was added|
| newValue | any   | the new value, or null if an item was removed|
| url*     | string| the page which called a method that triggered this change|
|* Note: the `url` property was originally called `uri`. Some browsers shipped with that property before the specification changed. For maximum compatibility, you should check whether the `url` property exists, and if not, check for the `uri` property instead.|
| | |

The storage event is not cancelable. From within the handle_storage callback function, there is no way to stop the change from occurring. It’s simply a way for the browser to tell you, “hey, this just happened. There’s nothing you can do about it now.

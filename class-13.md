# USING HTML5 STORAGE


HTML5 Storage is based on named key/value pairs. You store data based on a named key, then you can retrieve that data with the same key. The named key is a string. The data can be any type supported by JavaScript, including strings, Booleans, integers, or floats. However, the data is actually stored as a string. If you are storing and retrieving anything other than strings, you will need to use functions like `parseInt()` or `parseFloat()` to coerce your retrieved data into the expected JavaScript datatype.

```
interface Storage {
  getter any getItem(in DOMString key);
  setter creator void setItem(in DOMString key, in any data);
};
```

Calling `setItem()` with a ***named key*** that already exists will silently overwrite the previous value. Calling `getItem()` with a non-existent key will return **null** rather than throw an exception.


Like other JavaScript objects, you can treat the localStorage object as **an associative array**. Instead of using the `getItem()` and `setItem()` methods, you can simply use square brackets. For example, this snippet of code:

```
var foo = localStorage.getItem("bar");
// ...
localStorage.setItem("bar", foo);
…could be rewritten to use square bracket syntax instead:

var foo = localStorage["bar"];
// ...
localStorage["bar"] = foo;
```

There are also methods for removing the value for a given named key, and clearing the entire storage area (that is, deleting all the keys and values at once).

```
interface Storage {
  deleter void removeItem(in DOMString key);
  void clear();
};
```

Calling `removeItem()` with a non-existent key will do nothing.

Finally, there is a property to get the total number of values in the storage area, and to iterate through all of the keys by index (to get the name of each key).

```
interface Storage {
  readonly attribute unsigned long length;
  getter DOMString key(in unsigned long index);
};
```

If you call `key()` with an index that is not between 0–(length-1), the function will return null.

## TRACKING CHANGES TO THE HTML5 STORAGE AREA

If you want to keep track programmatically of when the storage area changes, you can trap the storage event. The storage event is fired on the window object whenever `setItem()`, `removeItem()`, or `clear()` is called and actually changes something. For example, if you set an item to its existing value or call `clear()` when there are no named keys, the storage event will not fire, because nothing actually changed in the storage area.


<hr>



## FURTHER READING
### ***HTML5 storage:***

HTML5 Storage specification
Introduction to DOM Storage on MSDN
Web Storage: easier, more powerful client-side data storage on Opera Developer Community
DOM Storage on Mozilla Developer Center. 


Internet Explorer Has Native Support for Persistence
Dojo Storage, part of a larger tutorial about the (now-defunct) Dojo Offline library
dojox.storage.manager API reference
dojox.storage Subversion repository

## Web SQL Database:

Web SQL Database specification
Introducing Web SQL Databases
Web Database demonstration
persistence.js, an “asynchronous JavaScript ORM” built on top of Web SQL Database and Gears
IndexedDB:

* Indexed Database API specification
* Beyond HTML5: Database APIs and the Road to IndexedDB
* Firefox 4: An early walk-through of IndexedDB
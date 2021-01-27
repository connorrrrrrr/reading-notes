# Local Storage

- cookies can be used for persistant local storage of small amounts of data.
- HTML5 storage is a way for web pages to store named key/value pairs locally, within the client web browser. 
- you can access HTML5 storage through the localStorage object on the global window object.
- in HTML5 storage, you store data based on a named key, then you can retrieve that data with the same key. The named key is a string. The data can be any type supported by javascript, including strings, booleans, integers, or floats.

- Like other JavaScript objects, you can treat the localStorage object as an associative array. Instead of using the getItem() and setItem() methods, you can simply use square brackets. For example, this snippet of code:
```javascript
var foo = localStorage.getItem("bar");
// ...
localStorage.setItem("bar", foo);
```
…could be rewritten to use square bracket syntax instead:
```javascript
var foo = localStorage["bar"];
// ...
localStorage["bar"] = foo;
```
- There are also methods for removing the value for a given named key, and clearing the entire storage area (that is, deleting all the keys and values at once).
```javascript
interface Storage {
  deleter void removeItem(in DOMString key);
  void clear();
};
```

[<===Home](README.md)
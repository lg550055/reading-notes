# Local Storage
HTML5 Storage provides local storage for web applications that persists beyond a page refresh with sufficient space.

It stores named key/value pairs:
- key is a string
- value is any JS type, stored as a string

***Since data is stored as a string, you have to parse retrieved data (e.g. `parseInt()`) to coerce it into the original JS type.***

### The localStorage object - an associative array

Be careful when setting or getting localStorage items:
- setItem() with a named key that already exists will **silently** overwrite the previous value
- getItem() with a non-existent key will return null rather than throw an exception

*Instead of setItem() and getItem(), you may use square brackets:
- localStorage['bar'] = foo;
- let foo = localStorage['bar'];

Additional methods:
- removeItem(key)
- key(index)
- clear()

### The storage event tracks changes
It fires on the window object when setItem(), getItem() or clear() is called **and** there are changes




---

[Back to table of contents](../README.md)
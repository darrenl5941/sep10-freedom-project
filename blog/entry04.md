# Entry 4: Learning a tool, jQuery
##### 03/02/2025

---

## Content

### What tool I chose

The tool I chose to learn is **jQuery**, which is a _tool_ or _library_ that is based on _JavaScript_. It allowes for more efficent use of _JavaScript_ by allowing you to do more with more simple and less coding or writing. It makes simple tasks that would take many lines of code into something you can call with only 1 line to make it work.

---

### Tinkering with jQuery

One example of me tinkering with _jQuery_ was when I made a basic function that would create the message, "I am great" that would appear when the webpage is first loaded. Here is the code:

``` js
$(document).ready(function() {

    $message = "I am great";
    test($message);

    function test($message) {

        alert($message);

    }

});
```

I then tried changing some things and tinkering around with the code. I changed the variable `message` to `hi` and make it print the message `"Hello world"`. Here is the code:

``` js
$(document).ready(function() {
    $hi = "Hello world";
    test($hi);



    function test($hi) {

        alert($hi);

    }

})
```

---

## Sources






















[Previous](entry03.md) | [Next](entry05.md)

[Home](../README.md)

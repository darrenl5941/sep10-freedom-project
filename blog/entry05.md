# Entry 5: Learning more about jQuery
##### 4/11/2025

## Content

### Parts of Functions

In _jQuery_ the main thing you can do is make _functions_ which can change parts of the webpage when specific things happen. The 3 main parts of a function are _selectors_, _events_, and _effects_ which I learned about in [an introduction to jQuery](https://www.digitalocean.com/community/tutorials/an-introduction-to-jquery).

**Selectors** are things that specify what to make the function effect or what object has the trigger to activate the function
* `$(“*”)` selects all elements
* `$(this)` selects current element being used in function
* `$(“p”)`: selects tags, in this case `<p>`
* `$(“.example”)` selects all elements with specified class
* `$(“#example”)` selects single unique elements with specified id
* `$("[type='text']")` selects any element with text applied to the type
* `$("p:first-of-type")` selects the first `<p>` in this case

**Events** are what needs to happen to the _selector_ for the function to trigger
* `click()` activates the function when the element is clicked
* `hover()` activates the function when your mouse is over an element
    * `mouseenter()` is the same as hover but only works when moving on the element
    * `mouseleave()`is also the same as hover but only works when moving the mouse off the element
* `submit()` activates when a selected form is submitted and it reloads the page
* `scroll()` activates the function when you scroll past a selected point on the specified element
* `keydown()` activates the function when a key on a keyboard is pressed

**Effects** specify what should happen to the selected element
* `toggle()` instantly swaps elements from visible to invisible or vise versa
    * `show()` makes selected elements visible if they are currently invisible
    * `hide()` makes selected elements invisible if they are currently visible
    * `fadeToggle()` does the same thing as `toggle()` but slowly makes the element fade away or into view
        * `fadeIn()` only does the appearing into view part of `fadeToggle()`
        * `fadeOut()` only does the fading out of view part of `fadeToggle()`
    * `slideToggle()` is the same as `toggle()`, but makes elements slide up/down when disappearing/appearing
        * `slideDown()` only does the appearing part of `slideToggle()`
        * `slideUp()` only does the disappearing part of `slideToggle()`
* `animate()` allows you to give a custom animation to the specified elements
* `css()` allows you to change the _CSS_ in the elements

---

### Making functions

I practiced _selectors_, _events_, and _effects_ that I learned by following a [jQuery Guide](https://www.youtube.com/watch?v=Q7Nwq7319X4) and trying to change around the code that it showed.

One of the functions I made changed the color of the background to red:

```js
$("#change-color").click(function() {
    $("body").css("background-color", "red");
});
```
When the element(s) with the specified id, `change-color`, are clicked the body will have its background color change to red.

---

While making functions some would have problems with clicking, so i learned and practiced with more advanced functions that used **DOM Traversal** so they would always work:
```js
$("body").on("click", "#dom", function(){
    alert($("ul").children().html());
});
```
This code checks inside the `body` for when the element(s) with the id `dom` are clicked to run the function. It makes sure that all the elements register the function so the code works.

---

I also tinkered with the selectors `"_:first-of-type"` and `"#_"` (id) because I didn't know the difference between them. I made one function for each:

```js
$("body").click(function() {
    $("p:first-of-type").css("color", "red");
});
```

```js
$("body").click(function() {
    $("#1").css("color", "red");
});
```

The first function which is for `"_:first-of-type"` works on every `p` that is the first `p` in its parent element. The other function which is for `"#_"` only works on 1 element which is the first one with the specified id.

## Skills

### Learning on My Own

To learn about _jQuery_ and how to use the functions it has I had to search it up on my own. I searched up the [different parts of functions](https://www.digitalocean.com/community/tutorials/an-introduction-to-jquery), and then searched up [a guide with examples](https://www.youtube.com/watch?v=Q7Nwq7319X4). Using these sources I further edited and experimented with the code to learn more about the functions I was using. This skill is

---

### Time Management

During the time between this entry and the previous one I learned more _time managment_ skills as I had to do a learning log every week. Because of this I had to manage my time better and make sure that I had the time to learn more about _jQuery_ every week instead of pushing it all to right before this entry. This skill is important because it makes sure that I give myself the appropriate amount of time needed to complete tasks.

[Previous](entry04.md) | [Next](entry06.md)

[Home](../README.md)

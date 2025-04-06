# Tool Learning Log

## Tool: **jQuery**

### 03/03/2025

* [jQuery Guide](https://www.youtube.com/watch?v=Q7Nwq7319X4)
  * Selectors
    * `.hide` allows you to hide or temporarily remove elements from the webpage
    * `.css` allows you to change the css that is used
      * In this case once the function is ran the background color of any `inputs` will turn red
      ``` js
      $(document).ready(function() {
        $("input").css("background-color", "red");
      });
      ```
      * Can be used to make the website change in some ways (color, etc) when something happens
    * `.click` allows you to do other functions when you click on an element
* [Bootstrap website](https://getbootstrap.com/docs/5.3/components/carousel/)
  * `carousel` allows you to make a slideshow that can cycle between different images
  * `navbar` A bar that stays on the top of your screen with links to different parts of your website
  * `card` It makes cards that hold information. They can be put in multiple columns

---

### 03/10/2025:

* [jQuery Guide](https://www.youtube.com/watch?v=Q7Nwq7319X4)
  * **Bubbling** sends an event from an element to it's parent and up the tree to make sure the event happens
    * An _example_ of this is show in the code snippet below, if it were to bubble, the event from the `div`with the `change-color` id would be sent to it's parent `div`, then the `body`, then the `html`.
      ```html
      <html>
        <body>
          <div>
              <div id = "change-color">
                  CLICK ME
              </div>
          </div>
        </body>
      </html>
      ```
     * The _javascript_ that allows for bubbling is made by setting it so the body does the action instead when the element with the tag you selected is clicked.
      ```js
      $(document).ready(function(){

        // bubbling
        $("body").on("click", "#change-color", function(){

          //stays the same
          $("body").css("background-color", "red");

        });
      });
      ```
  * **DOM traversal** is going through _elements_ to reach specific elements, Some things that is uses to do that are:
    * `children()` which gets all child elements of specific element
    * `each()` which gets specificed elements and does specified call back function
    * `find()` that gets all specified children elements of specified element
    * `next()` which takes the immediate next sibling of specified element
    * `parent()` which gets the parent of specified element
    * `prev()` which get the previous sibling of specified element
    * `siblings()` whcih takes siblings of specified element

---

### 03/17/2025:

* [Digital Ocean jQuery Guide](https://www.digitalocean.com/community/tutorials/an-introduction-to-jquery)
  * **Selectors** let you select what you want to do an action on
    * `$(“*”)` selects all elements
    * `$(this)` selects current element being used in function
    * `$(“p”)`: selects tags, in this case `<p>`
    * `$(“.example”)` selects all elements with specified class
    * `$(“#example”)` selects single unique elements with specified id
      * Only the `<h1>` element would turn blue because it selects the first element with the specified id
      ```html
        <h1 class="heading" id="id">Hello</h1>
        <p class="text" id="id">World</p>
        ```

        ```js
        $(document).ready(function() {

            $("#id").css("color", "blue");

        });
        ```
    * `$("[type='text']")` selects any element with text applied to the type
    * `$("p:first-of-type")` selects the first `<p>` in this case

---

### 03/24/2025:
* [Digital Ocean jQuery Guide](https://www.digitalocean.com/community/tutorials/an-introduction-to-jquery)
  * **Events** are the things that choose what needs to be done for something to happen, without it things would just happen instantly once the webpage is loaded
    * `click()` makes it so the action only happens when the specified object is clicked this means after the click is let go of
    * If you hold down your click the action will not happen untill you let go of it
      * In this example anything inside this function will only happen when the `body` is clicked
        ```js
        $("body").click(function() {

        });
        ```
    * `hover()` works when you hover your mouse onto or off of an object
      * If the `hover()` it involves an animation activating the hover too fast will lead to the animation backing up and repeating even after you stop hovering on and off
      * In this case going over the body would make the elements with `.class` dissapear and then reappear when going off the element, It also leads an element that dissapears that you are hovering over constantly dissapearing and reappering.
      ```js
        $("body").hover(function() {

            $(".class").fadeToggle();

        });
      ```
      * `mouseenter()` and `mouseleave()` split up `hover` so it only activates when you move your mouse on or off an element depending on which event.
    * `submit()` causes the effect to happen when a form is submitted



  * **Effects** are the code that say what should happen and udner what conditions they should happen
    * `toggle()` causes whatever is selected to turn visible if invisible and invisible if visible
      * In this case whenever the `body` is clicked anything with `.class` will turn from visible to invisible or vise versa.
        ```js
        $("body").click(function() {

            $(".class").toggle();

        });
        ```
      * `fadeToggle()` does the same thing as `toggle()` but adds a fading in/out animation
        * `fadeIn()` and `fadeOut()` do the same thing as fade toggle but only allow for one part, either fading in, or out, not both

---

### 3/31/2025:
* [Digital Ocean jQuery Guide](https://www.digitalocean.com/community/tutorials/an-introduction-to-jquery)
  * **Effects**:
    * `slideToggle()` makes all the selected elements go up and vanish if they are visible or go down and reappear if they are invisible
      * With this code clicking the `body` will cause anything with `.class` tp toggle, but with an animation making them all slide up or down.
        ``` js
        $("body").click(function() {

            $(".class").slideToggle();

        });
        ```
      * `slideUp()` makes the elements vanish by sliding upwards
      * `slideDown()` makes the elements reappear by sliding downwards

---

### X/X/XX:
* Text


<!--
* Links you used today (websites, videos, etc)
* Things you tried, progress you made, etc
* Challenges, a-ha moments, etc
* Questions you still have
* What you're going to try next
-->

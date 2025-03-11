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

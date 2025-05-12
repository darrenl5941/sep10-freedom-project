# Entry 6: Making my MVP (Minimum Viable Product)
##### 05/12/2025

## Content

### Making a Plan

Before starting to make by website I started by making a plan. I first made multiple **wireframes** to plan out how my website should look for different screen sizes. Although I changed some things from how I planned it out in my wireframe it was important for me to make wireframes because it gave me a base for how I wanted it to look, and it saved me time from having to change everything and moving around more complex elements because I already knew where I wanted everything.

#### Mobile Wireframe:

![1st half of Mobile Wireframe](../prep/wireframes/mobile-wireframe-1.png)
![2nd half of Mobile Wireframe](../prep/wireframes/mobile-wireframe-2.png)

#### Computer Wifeframe:

![Computer Wireframe](../prep/wireframes/computer-wireframe.png)

### Making the MVP for my Website

While making the MVP for my website I followed multiple steps I made for myself and planned how long each would take:

* make divs & layout - 4/28
    * In this part I looked at what my _wifeframe_ looked like and coded all my sections to look like it
* add content/text onto webpage - 4/29
    * I took the notes and other things that I already had planned out and _pasted it onto the website_ as well as adding some new information
* add bootstrap - 5/2
    * I added my _navbar_ and other _bootstrap components_ as I already made the _rows and columns_ I needed for the layout
* add images - 5/2
    *I took the images I save as well as new ones and then imported it into Github and then put the _inline links_ to them inside the webpage
* add colors - 5/3
    * I put in backgrounds for the colors and different sections to make my website look nicer
* add basic interactions with jQuery - 5/3
    * I used what I learned from jQuery to add things such as swapping sections by clicking

### Challenges

#### Challenge 1

One challenge that I had while making by website was the _padding_ for my images now working properly. When I made my images they had padding around them and I didn't know why. The problem was that a previous class t hat I had made was also giving the images padding:

``` css
.div-col, .div-img {
    border: black, 5px, solid;
    padding: 5px;
}
```

To fix this I made a new class for all my images that had `!important` so it would take place over the previous class which I still needed to work on other parts of the website:

``` css
.logo, .monitor-image, .hardware-image, .future-technology-image {
    padding: 0px !important;
}
```

#### Challenge 2



[Previous](entry05.md) | [Next](entry07.md)

[Home](../README.md)

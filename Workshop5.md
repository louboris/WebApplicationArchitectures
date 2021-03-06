# Web Application Architectures WorkShop 5 : Canvas, JS, localStorage

## Web Application Architectures COURSE SYLLABUS

1. Web Infrastructure  
Internet History, Cables, TCP/IP, HTTP, CLIENT/SERVER, NETCAT

2. Web Fundamentals 1/2  
HTML / CSS / LOCAL WEB SERVER / RESPONSIVE 

3. Web Fundamentals 2/2  
Box model, Fonts, Basic JS, DOM, InnerHTML, DOM Events, Event Handlers
getElementById

4. CSS Animations

5. Canvas / JSON / Local Storage

6. Node.JS / REST API / Fetch / Promises

7. Database Access

8. React

9. React

10. Deployment

***

## WS 4.1 Assignement Correction

***

## WS 5.1 Let's Draw using CANVAS and JS, and work with data using localStorage

To draw graphics on the fly in your browser you are face with two options: **SVG** vs **Canvas**  
- SVG is a standard for vector graphics. you will use a language to describe 2D graphics in XML.
- Many vector graphics software can export visual figures as svg that can be copy/pasted in your code.
Inkscape, boxysvg, vectr.com ...
- SVG figures are elements within the DOM, you can use javascript on them, and CSS animations.

- With Canvas, you setup a space, and then you write javascript to draw and animate.
- Figures within a CANVAS are just pixels. They have no representation in the DOM. Only your canvas is a DOM object.


**If you want to know more about svg vs canvas:**  
https://css-tricks.com/when-to-use-svg-vs-when-to-use-canvas/


**Must Read:**  

https://www.w3schools.com/html/html5_canvas.asp  
https://www.w3schools.com/html/html5_svg.asp



**Fast Tutorial:**  
https://www.digitalocean.com/community/tutorials/js-drawing-shapes-canvas-api

**Medium length Tutorial**  
https://www.w3schools.com/graphics/canvas_intro.asp

**Long Tutorial:**  
https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial


**Assignement :**

Create a webpage with (from top to bottom):  
- A title
- A control bar (just a space with buttons)
- A drawing box (just an empty space)

The control bar will contain : 

- A dropdown menu to choose a form among square, triangle, circle.
- A HTML color picker ( `<input type="color">` ) to choose a bgcolor (choose your palette )
- A HTML color picker ( `<input type="color">` ) to choose a border color (choose your palette )
- A dropdown menu to choose the border thickness ( 2;4;6;8;10;20 px)
- A dropdown menu to choose figure size (20;40;60;80;100;200 px)
- A button that will display the specified figure and place it at a random place on the viewport.


Instructions :  
- Every button and color picker must have its label
- All colors are black by default
- Webpage must work well on mobile.
- Dropdown menu are easy to implement using `<SELECT></SELECT>`
- put your code on codepen and send me a private zoom message when done
- Beware of canvas size and resolution, they are different  
canvas have a default resolution of 300x150, so if you specify a bigger size in your css, pixel will be stretched, giving your figures ugly borders.  
https://riptutorial.com/html5-canvas/example/7515/canvas-size-and-resolution



**v1.1** : Store all created figure data using localStorage. when you close and re open your browser, figures re-appear at random position

A javascript Object seem to be the simple way to store your figures specifications.  
But you can only store key:value pairs in localStorage  
One solution is to stringify your Object :  
https://stackoverflow.com/questions/2010892/storing-objects-in-html5-localstorage  

**Must Read for v1.1:**  
https://www.w3schools.com/jsref/prop_win_localstorage.asp


**v1.2** : The figures must never overlap with viewport borders. every figure should fit in the screen.  

**2D Collision detection tutorial:**
https://developer.mozilla.org/en-US/docs/Games/Techniques/2D_collision_detection


**v1.3** : The figures must never overlap with other figures.   

**v1.4** : Let's make this visually nice, and avoid clashing colors, by restricting all our color pickers to a predefined color palette.
use https://coolors.co/ to generate a 5 colors palette. Use `<datalist>` to restrict your color picker.  

**v1.5** : Create a new button that generate 10 random figures upon each click

**PROPOSE IDEAS FOR IMPROVEMENT**

## FOR OUR NEXT WORSHOP : 

- Finish 5.1 

- Read Workshop6.md, Watch the event loop video, Read the pdf on Fetch and Promises. I will ask random questions at the beginning of the Worskhop to make sure all of you watched and read the content. IF you want to learn while watching the video, I advise you to take notes.


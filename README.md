## Website Performance Optimization portfolio project
----------------------------
## About
The purpose of this project is to optimize this online portfolio for speed In particular, optimize the critical rendering path and make this page render in speed of at least 90 scores for both mobile and desktop view for `index.html` and run `pizza.html` at 60fps when scrolling.

---------------------------
### Getting started
in order for you to run this site :
1- you can download all the files from [my repo](https://github.com/xxiMiaxx/frontend-nanodegree-mobile-portfolio) and open `index.html` in your web browser.
2- or you can just [click here](https://xximiaxx.github.io/frontend-nanodegree-mobile-portfolio/)
---------------------------
#### Changes made to optimize this site :

#### Part 1: Optimize PageSpeed Insights score for index.html
1- use `async` attribute to stop JS from blocking the rendering path by synchronously loading low priority scripts.
2- place the function inside `<script>` at the bottom of the `<body>`
3- inline the external `style.css` file to ensure that the css is not render blocking and to dekiver the styling as quickly as possibale.
4- remove the web font as it can slow the page down.
5- compress the images to reudce their size.
6- resize the pizza image.
7- use media querie `media="print"` for the external `print.css` sheet as you don't need it to load every time you open the page unless you are planning on printing.
8- minifiy the `print.css` sheet.
---------------------------

#### Part 2: Optimize Frames per Second in pizza.html
1- take al the `var` declerations out of loops.
2- take some calculations out of loops as we don't need them to recalculate with every iteration when the reult is always the same.
3- turn the `sizeSwitcher` switch statment into a flat object data structure.
4- use the `requestAnimationFrame` methode to make sure that `updatePositions` code is called when the users computer is ready to make changes to the screen each time, which reults in a smoothe more efficient animation.
5- compress all images.
6- minify JS and CSS files.
7- change every `querySelector` with `getElementById` cause it's faster.
8- save the array length in a varibale `pLength`, so the value isn't checked with every iteration.
---------------------------
### Results

##### Desktop `index.html` score :
93/100
   ![](https://github.com/xxiMiaxx/frontend-nanodegree-mobile-portfolio/blob/master/screenshots/Screen%20Shot%202017-10-20%20at%206.34.21%20PM.png)
##### Mobile `index.html` score :
91/100
![](https://github.com/xxiMiaxx/frontend-nanodegree-mobile-portfolio/blob/master/screenshots/Screen%20Shot%202017-10-20%20at%206.36.50%20PM.png)
### Resources & Tools:
* [page speed insight](https://developers.google.com/speed/pagespeed/)
* [for image optimizing](http://optimizilla.com/)
* [Markdown guidlines](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
* [JavaScript minifier](https://javascript-minifier.com/)
* [CSS minfier](https://cssminifier.com/)
* [JS beautifier](http://jsbeautifier.org/)
* [pic resize](http://picresize.com/)
* [GitHub pages](https://pages.github.com/)

Website Optimization Project
===============================


### Project Description

To optimize a provided website with a number of optimization- and performance-related issues so that it achieves a target PageSpeed score of 90 and runs at 60 frames per second.

### Setting Up the Application

Clone the repo https://github.com/AN1TAMARY/weboptimization.git.
And your repository will include the following files
1 index.html - Contains html for the main page in the browser.
2 project-2048.html/project-mobile.html/project-webperf.html - Contains html for the various pages of the website.
3 css folder - Contains css relevant to the main page. These files include print.css and style.css. Note - style.css was inlined in index.html, as it continually caused render blocks. The file then, is no longer called by index.html.
4 js folder - Conatins javascript files relevant to the main page. 
5 img folder - Contains all images for the main page.
6 views folder - Contains all files relevant to the 'Cam's Pizzeria' page. The views folder contains the following files:
i) pizza.html - Conatins html for the pizzeria page.
ii)css folder - Contains bootstrap-grid.css and styles.css
iii)images folder - Contains the images for the pizzeria page.
iv)js folder - Contains the main.js file which manages the main functionality of the pizzeria app.

### Optimization list

Main Page
1 Print css file was given a media tag so it would only apply when the user attempts to pring the page.
2 A script was included into index.html which asynchrously loads the fonts obtained by Google Fonts.
3 All styles from the original style.css were inlined - the file was small enough to where it would drastically reduce render blocking CSS.

Pizzeria
1 querySelectorAll('id') were replaced in favor of document.getElementbyId('id')
2 Calculations that could be removed from iterations and stored instead were moved.
3 The number of pizzas moving in the background were reduced.
4 Request Animation Frame functions were utilized to improve the performance of the sliding background pizzas.
5 translatX() were used to improve animation times.

Minification
Files were minified to reduce their load times using grunt.
Images were also optimized.
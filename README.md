## Website Performance Optimization portfolio project

### Instructions
To view the portfolio website, download and upzip all the files and open index.html in your browser.
To view the pizza website, download and unzip all of the files and open views/pizza.html in your browser.

####Part 1: Optimize PageSpeed Insights score for index.html
*Minify CSS and placed into head. Add media tag for print.css
*Change JS loading to async.
*Resize and compress the images. 

####Part 2: Optimize Frames per Second in pizza.html

*Changed all querySelector to the faster methods of accessing our specified DOM elements, i.e. getElementById and getElementByClassName. 

*Declared variables to store the needed DOM elements so that the browser isn't repeatedly querying the DOM every time in the for loops, in the updatePositions and changePizzaSizes funcitons

*Moved the document.body request out of for loop in the changePizzaSizes and updatePositions functions. This prevents the browser from having to render the page every time the loop iterates.

*Instead of setting an arbitrary upper bound for i in the for loop of appending image to movingPizzas1, we calculate the number of pizzas needed to fill the webpage based on browser inner dimensions.

In order to reduce the paint time, "backface-visibility: hidden" has been added to the CSS for the "mover" class.
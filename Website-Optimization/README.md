## Website Optimization

### Steps to open the file
open index.html in your browser.

To view the pizza website download all of the files and open views/pizza.html in your browser.


## Optimizations

* Modified the code to calculate the number of pizzas needed to fill the webpage based on browser inner dimensions.

* Moved the document.body request out of for loop in the changePizzaSizes and updatePositions functions. This prevents the browser from having to render the page every time the loop iterates inn pizza.html.

* Bootstrap grid used instead of using style attribute for better performance in both index.html and pizza.html

* Used internal css instead of external css.

* Cached the needed DOM elements so that the brower isn't querying the DOM every time the for loops are iterated in the updatePositions and changePizzaSizes funcitons

* Changed all instances of querySelector to the more efficient getElementById and getElementByClassName depending on whether a class or id is needed.

* In changePizzaSizes function an additional array mynewWidth to optimize the rendering of page and grouping all DOM elements together and rendering in different loop.
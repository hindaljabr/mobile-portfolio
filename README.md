## Website Performance Optimization portfolio project
This is the project 6 of the FEND program.
It's about website optimization.
Objectives:
- Optimize the critical rendering path for "index.html" page.
- Optimize the browser rendering for "Cam's Pizzeria" page.

### Getting started

#### What You Need
Any web browser.

#### Run the Webpages
1. Download the github zip file, unzip it.
2. Open *index.html* in your browser.
3. Open *Cam's Pizza* page in your browser.


### My Changes to the Existing Code
*Main page*: is optimized, images are optimized.

*Main js file*:
- Stored document.querySelectorAll() so it doesn't have to be called in each iteration.
- Moved setting of style.width to a separate loop.
- Replaced style.left with style.transform.
- Removed pizzas that we never seen from the Render Tree.
- Moved body.scrollTop out of the loop.
- Replaced expression using modulo operator with a simple counter var.

### Changes after review
- Optimized pizza.png.
- Created a local var randomPizzaContainer outside the loop so the DOM is not explicitly touched in every iteration.
- Removed dx and newwidth outside the loop since its a static value.
- Removed movingPizzas outside the loop and added movingPizzas.appendChild(elem) inside the loop.

### Changes after 2nd review
- Changed the [i] to [0] in determineDx.

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
*Main page*: is optimized to speed score of at least 90/100 for Mobile and Desktop.

*changePizzaSlices Function*:
- Stored document.querySelectorAll() so it doesn't have to be called in each iteration.
- Moved setting of style.width to a separate loop.

*updatePositions Function*:
- Replaced style.left with style.transform.
- Removed pizzas that we never seen from the Render Tree.
- Moved body.scrollTop out of the loop.
- Replaced use of querySelectorAll() with getElementsByClassName().
- Replaced expression using modulo operator with a simple counter var.

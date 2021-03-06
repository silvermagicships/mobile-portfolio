## Website Performance Optimization portfolio project

This was the 4th Udacity project in the Frontend Web Developer Nanodegree program. The challenge was to optimize an online portfolio site for speed and, in particular, to optimize the
critical rendering path and make the page render as quickly as possible by applying the techniques picked up in the [Critical Rendering Path course](https://www.udacity.com/course/ud884).


### Getting started

####Part 1: Optimize PageSpeed Insights score for index.html

Steps to load the project:

1. Type `git clone https://github.com/silvermagicships/mobile-portfolio.git` in your command line
1. Run a local server

  ```bash
  $> cd /path/to/mobile-portfolio
  $> python -m SimpleHTTPServer 8080
  ```

1. Open a browser and visit localhost:8080
1. Download and install [ngrok](https://ngrok.com/) to make your local server accessible remotely.

  ``` bash
  $> cd /path/to/your-project-folder
  $> ngrok http 8080
  ```

Copy the public URL ngrok gives you and try running it through [PageSpeed Insights](https://developers.google.com/speed/pagespeed/insights/).
To inspect different elements on the page and to record a timeline, you can use Chrome DevTools.

How to run tasks with Grunt:

1. Install Node.js and npm
2. Install grunt 
3. Create a package.json file
4. Install all relevant plugins
5. Create grunt file
6. Configure tasks
7. Run the command 'grunt' in your command line


Optimizations done:

* Made style.css inline
* Minified print.css with Grunt and added media type
* Uglified perfmatters.js with Grunt and made it run asynchronously
* Made analytics.js run asynchronously
* Made web fonts run asynchronously
* Minified HTML with Grunt
* Moved all scripts to the bottom of the doc
* Optimized pizzeria.jpg with imagemagick

Tools used:

* Grunt
* imagemagick

####Part 2: Optimize Frames per Second in pizza.html

To optimize views/pizza.html, you will need to modify views/js/main.js until your frames per second rate is 60 fps or higher. 

Optimizations done:

* Inlined style.css in pizza.html
* Optimized loop for changePizzaSizes function by declaring variables outside of the loop
* Used getElementsByClassName instead of querySelectorAll to increase speed
* Optimized for loop for updatePositions function by declaring variables outside of the loop
* Used getElementsByClassName instead of querySelectorAll to increase speed
* Optimized for loop for generating sliding pizzas when the page loads by declaring variables outside of the loop
* Used getElementById instead of querySelector to increase speed



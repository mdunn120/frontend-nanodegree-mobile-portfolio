## Website Performance Optimization portfolio project

##Installation and Usage
###Part 1A
1. Clone the repository to your computer
2. Drag and Drop index.html into the Chrome browser
3. Press the refresh button in the Chrome browser and you will see that this page loads very quickly.
###Part 1B
1. Install python on your computer
2. Install ngrok on your computer
3. Create a website URL that will be able to run in the PageSpeed Insights website by using the python
and ngrok commands below in the Instructions for Project
4. Take the URL given to you by ngrok and put it into the PageSpeed Insights page
5. Notice that both Mobile and Desktop have PageSpeed Insights over 90!
###Part 2A
1. Drag and drop pizza.html into the chrome browser
2. Scroll the page and notice how buttery smooth the scrolling is
###Part 2B
1. In the chrome browser go to chrome://inspect/#pages and insect the pizza.html page
2. Scroll the pizza.html page while recording the data in the chrome inspect tool and notice that pizza.html is rendering at 60fps. 
###Part 2C
1. Scroll down to the resize Pizza slider 
2. Record Timeline information with the Chrome inspect tool of changing the pizza size slider. Notice that Time to resize pizzas is less than 5 ms using the pizza size slider.

##Main things I did in the project
###Part 1: PageSpeed Score: Critical Rendering Path - index.html achieves a PageSpeed score of at least 90 for Mobile and Desktop.
1. Took out the font call
2. Defer the analytics script in index.html
3. Compressed pizzeria.jpg and profilepic.jpg using the compression image menu in Office Powerpoint 
4. link async href="css/print.css" rel="stylesheet"
5. Inline the css
###Part 2: Getting Rid of Jank: Frame Rate, Computational Efficiency
1. Took modulo calcualtions out of the for loop of layout
2. Changed 200 rendered Pizzas to 22. I still have the same effect
	Super helpful video: https://classroom.udacity.com/nanodegrees/nd001/parts/00113454012/modules/273584856175462/lessons/5988439100/concepts/68776485930923
3. 
		
#Instructions for Project
Your challenge, if you wish to accept it (and we sure hope you will), is to optimize this online portfolio for speed! In particular, optimize the critical rendering path and make this page render as quickly as possible by applying the techniques you've picked up in the [Critical Rendering Path course](https://www.udacity.com/course/ud884).

To get started, check out the repository and inspect the code.

### Getting started

####Part 1: Optimize PageSpeed Insights score for index.html

Some useful tips to help you get started:

1. Check out the repository
1. To inspect the site on your phone, you can run a local server

  ```bash
  $> cd /path/to/your-project-folder
  $> python -m SimpleHTTPServer 8080
  ```

1. Open a browser and visit localhost:8080
1. Download and install [ngrok](https://ngrok.com/) to make your local server accessible remotely.

  ``` bash
  $> cd /path/to/your-project-folder
  $> ngrok http 8080
  ```

1. Copy the public URL ngrok gives you and try running it through PageSpeed Insights! Optional: [More on integrating ngrok, Grunt and PageSpeed.](http://www.jamescryer.com/2014/06/12/grunt-pagespeed-and-ngrok-locally-testing/)

Profile, optimize, measure... and then lather, rinse, and repeat. Good luck!

####Part 2: Optimize Frames per Second in pizza.html

To optimize views/pizza.html, you will need to modify views/js/main.js until your frames per second rate is 60 fps or higher. You will find instructive comments in main.js. 

You might find the FPS Counter/HUD Display useful in Chrome developer tools described here: [Chrome Dev Tools tips-and-tricks](https://developer.chrome.com/devtools/docs/tips-and-tricks).

### Optimization Tips and Tricks
* [Optimizing Performance](https://developers.google.com/web/fundamentals/performance/ "web performance")
* [Analyzing the Critical Rendering Path](https://developers.google.com/web/fundamentals/performance/critical-rendering-path/analyzing-crp.html "analyzing crp")
* [Optimizing the Critical Rendering Path](https://developers.google.com/web/fundamentals/performance/critical-rendering-path/optimizing-critical-rendering-path.html "optimize the crp!")
* [Avoiding Rendering Blocking CSS](https://developers.google.com/web/fundamentals/performance/critical-rendering-path/render-blocking-css.html "render blocking css")
* [Optimizing JavaScript](https://developers.google.com/web/fundamentals/performance/critical-rendering-path/adding-interactivity-with-javascript.html "javascript")
* [Measuring with Navigation Timing](https://developers.google.com/web/fundamentals/performance/critical-rendering-path/measure-crp.html "nav timing api"). We didn't cover the Navigation Timing API in the first two lessons but it's an incredibly useful tool for automated page profiling. I highly recommend reading.
* <a href="https://developers.google.com/web/fundamentals/performance/optimizing-content-efficiency/eliminate-downloads.html">The fewer the downloads, the better</a>
* <a href="https://developers.google.com/web/fundamentals/performance/optimizing-content-efficiency/optimize-encoding-and-transfer.html">Reduce the size of text</a>
* <a href="https://developers.google.com/web/fundamentals/performance/optimizing-content-efficiency/image-optimization.html">Optimize images</a>
* <a href="https://developers.google.com/web/fundamentals/performance/optimizing-content-efficiency/http-caching.html">HTTP caching</a>

### Customization with Bootstrap
The portfolio was built on Twitter's <a href="http://getbootstrap.com/">Bootstrap</a> framework. All custom styles are in `dist/css/portfolio.css` in the portfolio repo.

* <a href="http://getbootstrap.com/css/">Bootstrap's CSS Classes</a>
* <a href="http://getbootstrap.com/components/">Bootstrap's Components</a>

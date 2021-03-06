# Jewel Clicker
A simple game I wrote as a project for class. Its main purpose is to show the usage of hit regions in the HTML5 `canvas` object.
## How to Play
### Prerequisites
Since this game uses the canvas, in order to play it, you obviously need to be using a browser that supports the Canvas element. Fortunately, there's an easy way to check that; any content within the `canvas` tag is printed to the screen only if the `canvas` itself can't be shown. Usually, this is a "your browser doesn't support this" message. If you see this message, you're most likely running an old version of Internet Explorer, so you should use that for what it's best at; downloading a real browser.

Once you're able to see the canvas, you'll need to enable hit regions. Since this is still in development, it's hidden behind developer flags. In Firefox, go to `about:config` and set `canvas.hitregions.enabled` to `true`. In Chrome, go to `chrome://flags` and set ExperimentalCanvasFeatures to true. Once you've done that, go to [this page](http://www.rgraph.net/blog/2013/january/html5-canvas-hit-regions.html) and make sure "your browser" has the feature working.
### Gameplay
At the start of the game, all jewels are transparent and spinning, with random colors assigned to them. Clicking on one changes its color to another random one. If the color it changes to is the same as the color of a jewel next to it, both will freeze and form a group. This effect will spread recursively to freeze all same-colored jewels any jewel in the group is touching. Once a jewel is frozen, you can't click on it anymore. The biggest group will become solid, and your score is directly proportional to the size of the biggest group. How many jewels can you get into a group before it's surrounded by other groups and stopped from growing any further? 

Credit for the jewel images used goes to qubodup on [opengameart](http://opengameart.org/content/rotating-crystal-animation-8-step).
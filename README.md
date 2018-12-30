# A Christmas Letter from the CEO

This is a HTML file that has a placeholder for message body and a signature image at the end. The background is generated and animated via JavaScript.

## HTML/CSS
The HTML has a foreground upon which the message text is displayed. There is a background for the animation. The two divs are styled using *foreground* and *background* respectively. Both have the *display* property set to *absolute* and take up the whole of the screen. *foreground*'s *z-index* property will naturally be higher than that of *background*.

There are 12 divs in *background*. Each div is styled using *snowflake*. 6 of these are also styled using *left*, while the other 6 are styled using *right*.

## JavaScript
On load, the *initSnowflakes()* function is called. This will giv each *snowflake* div a background image randomly generated, and set the initial height and width to 100 pixels.

*transitSnowflakes()* will position each *snowflake* div left or right of the screen depending on whether they are styled *left* or *right*. It will also set certain properties at random, such as...
- height and width
- rotation
- transition speed
- position from top and left/right of screen

*transitSnowflakes()*  is called after the *initSnowflakes()* call, and every time the page is scrolled.


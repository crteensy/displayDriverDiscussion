Color Spaces
=

Identified color spaces used in an application:
- The display's native color space. Sometimes this can be configured, sometimes not. Configuring the display's color system and propagating it to the canvas is done by the display driver.
- The canvas' color space. This is how color information is stored by the canvas.
- How the application passes color information to drawing functions. In an ideal world, any color argument can be converted to canvas color space

So if a display is RGB16, the canvas is RGB24, and a drawing function is simply given a 'true' color (meaning white), this should automatically be converted to RGB16 on its way to the display.
The conversion from any Color to any other Color should be done as efficiently as possible.

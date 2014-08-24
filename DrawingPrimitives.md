Drawing Primitives
=

When something is drawn, the color needs to be specified. This is the canvas' own color type, which should be configurable. In the signatures below, the color argument is called c.

Coordinate Arguments
-

Coordinates are sometimes passed as x and y arguments, and sometimes a point type is passed. Passing a point (reference) might be more efficient.

Mandatory Drawing Primitives
-

The common display drivers have
- drawPixel(x,y,c),
- drawLine(x0,y0,x1,y1,c)
- drawEllipse(x,y,width,height,c)
- drawCircle(...) as a wrapper for drawEllipse with widht=height
- drawFrame(x0,y0,x1,y1,c) or drawRect(x0,y0,x1,y1,c)
- drawVLine(x,y,h,c)
- drawHLine(x,y,w,c)
- clear(c) clears all screen using fill or clear(x0,y0,x1,y1,c) clear a portion

Sometimes an option for filling ellipses and frames is added, either as a parameter or as a separate function.

Optional Drawing Primitives
-

Less common are
- drawTriangle(x0,y0,x1,y1,x2,y2,c)
- drawPolygon(...,c)
- drawArc(x,y,r,r-start,r-end,color)
- drawRoundRect(x,y,w,h,r,c)
- drawBitmap(...)

again, these might have a fill option or a separate function that fills the drawn shape.

Characters and Strings
-

It should be possible to choose between different fonts, from different sources:
- Flash,
- RAM,
- a display's native fonts (if it provides any).

Functions:
- drawChar(x0,y0,char,c)
- drawString(x0,y0,string,c)<br>
used in with Print...
- Print("xxx");
- Println("xxx");
- write(char);

Further functions or classes should be supplied that can retrieve information about character and string geometry

Optional Character and String functions:
- A way to set the baseline
- center, flush left, and flush right
- wrap
- setTextColor(c) or setTextColor(foreground c, background c)
- setTextSize(...) maybe not if ext font used (fixed font) useful only for internal ASCII
- setTextRotation(...)
- setCursor(r,c) should divide the screen in row and column based on char selected


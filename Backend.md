Backend
=

The "Backend" is responsible for anything that happens between the canvas and the display driver.
If a display already implements _all_ functionality the canvas offers, the backend doesn't do much more than:

- Wait until the display driver reports that the display is not busy executing previous commands
- Tell the display driver when a new frame is drawn
- Tell the application to start drawing on the canvas

This is still a bit fuzzy.

If the display requires paging and/or color space conversion buffering in RAM, this is done by the backend.

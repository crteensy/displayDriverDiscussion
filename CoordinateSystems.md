Coordinate Systems

From high level to low level
- canvas: The coordinate system used by the application code to draw on the canvas.
I think this can be fixed to: x from left to right, y from top to bottom.
- physical: this can be different from both the native and the canvas coordinate system,
because the display might be rotated or be equipped with additional optics that mirror the image.
- native: The display's native coordinate system.

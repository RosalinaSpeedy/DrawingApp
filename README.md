# DrawingApp
Computing project 1 drawing app - made in collaboration with https://github.com/chewkel/chewkel.github.io 

Features implemented.
Ben – Curve, flood fill, select tool.
Curve tool.
Draws a rough guideline by dragging the mouse which is then smoothed into a curve. There is also an
option to edit points highlighted on the curve. Once completed, clicking away finalizes and bakes the
curve into the canvas. The tool is based on an array of coordinates system with editable points at
index % 5 and the start and end points. The object then enters a state to enable editing of individual
points by setting boolean values and recalling the function to draw the curve: replacing the old
coordinates in the array system.

Possible improvements for this tool include allowing for the user to extend their curve or delete
points from their curve (by holding down shift and clicking either on other points of the canvas or
points on the curve respectively); or introducing a system where curves need to have a minimum
distance between two points before logging the coordinates to the array (could be achieved using
the dist() function to compare points before pushing) to prevent creating a curve on a single point by
holding down the mouse in one spot.

Flood fill.
Fills a section of a specific colour on the canvas with the selected colour.

Select tool.
Draws a red selection box by dragging the mouse. The user can click and drag the selection to move
it around – or on one of the four corner knobs to resize and reshape it. Clicking outside the selection
will remove the selection box and bake the current state into the canvas.

This tool is based on using a p5JS image value to store the selection and resizing and redrawing it as
appropriate to match the user’s inputs.

Currently, dragging the selection over itself while resizing does not reverse the image as one might
expect, rather just keeps the orientation of the image but on the opposite side; therefore,
introduction of mirroring the selection by dragging it over itself is a possible improvement.

# DrawPad
Application created for personal use.  Rudimentary drawing software implemented using Java Swing, with the feature to export the drawing into code that can be pasted into other Java Swing projects.  Originally created March 2018.

In CS21B, we had to create an animated Greeting Card using the graphics functionality of Java Swing.
I created this DrawPad for personal use in this project so that I can make sophisticated shapes with a (mostly) intuitive GUI then easily export it into copy-pasteable code for the project.

Code is output to the Print folder, while works in progress are stored in the Save folder.

Features include:

Drawing:
- Multiple layers that are independent of each other.
- Each layer is responsible for a single polyline of a single color.  The curve may be filled in to form a polygon.
- Clicking on the DrawPad adds a new point to the end of the current layer's polyline.  Clicking and dragging is supported. 
- Color is decided either by an "eye-dropper" tool or directly inputting the RGB value
- The polyline's outline and the the polygon's fill can have separate colors.
- You can translate the position of the active polygon some number of pixels NSEW.
- You can translate all polygons at the same time.
- Redo and Undo functionality.  An "action" is the set of points between when the mouse is clicked and when it is released again.
- You can hide the current polygon (but not delete it)
- You can delete the current polygon
- You can show or hide the precise points on the polyline (these will still not be exported).

File Management:
- Save your current work
- Load previous work
- Output the current drawing into code that can be copy pasted into Java Swing to be rendered.

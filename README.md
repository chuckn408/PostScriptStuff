# PostScriptStuff

Just a small collection of my postscript notes

--Postcript files in .ps
--files are run through GhostScript

https://ghostscript.com/releases/gsdnld.html

First reference site::
https://paulbourke.net/dataformats/postscript/

Some other useful Commands::

**arc** 	- 
Draws an arc (including a circle). The arguments are xcenter, ycenter, radius, start angle, stop angle. The arc is drawn counterclockwise, the angles are in units of degrees.

**currentpoint** 	-  	
This is an example of an instruction that takes no arguments but leaves numbers on the stack, namely the coordinates of the current point.

**setdash** 	-  	
This sets the dash attribute of a line in terms of a mark-space array. Just as strings are denoted by round braces (), arrays are denoted by square braces []. For example the following command "[3 3] 0 setdash" would make any following lines have a 3 unit dash followed by a 3 unit space. The argument after the dash array is the offset for the start of the first dash.

**setlinecap** 	-  	
This specifies what the ends of a stroked line look like. It takes one argument which may be 0 (butt caps), 1 (round caps), or 2 (extended butt caps). The radius of round caps and the extension of the butt caps is determined by the line thickness.
	
**setlinejoin** 	-  	
This determines the appearance of joining lines. It takes one argument which may be 0 (miter join), 1 (round join), or 2 (bevel join).

**curveto** 	-  	
This draws a bezier curve defined by the three points given as arguments. The curve starts at the current point, ends at the last point, and the tangents are given by the line between the first-second and second-third pair.

**save and restore** 	-  	
Instead of having to "undo" changes to the graphics state it is possible using save to push the entire graphics state onto the stack and then reinstate it later with a restore. 

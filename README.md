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


Paper sizes

Paper Size                      Dimension (in points)
------------------              ---------------------
-Comm #10 Envelope-------------->297 x 684

-C5 Envelope-------------------->461 x 648

-DL Envelope--------------------->312 x 624

-Folio-------------->595 x 935

-Executive-------------->522 x 756

-Letter-------------->612 x 792

-Legal-------------->612 x 1008

-Ledger-------------->1224 x 792

-Tabloid-------------->792 x 1224

-A0-------------->2384 x 3370

-A1-------------->1684 x 2384

-A2-------------->1191 x 1684

-A3-------------->842 x 1191

-A4-------------->595 x 842

-A5-------------->420 x 595

-A6-------------->297 x 420

-A7-------------->210 x 297

-A8-------------->148 x 210

-A9-------------->105 x 148

-B0-------------->2920 x 4127

-B1-------------->2064 x 2920

-B2-------------->1460 x 2064

-B3-------------->1032 x 1460

-B4-------------->729 x 1032

-B5-------------->516 x 729

-B6-------------->363 x 516

-B7-------------->258 x 363

-B8-------------->181 x 258

-B9-------------->127 x 181

-B10-------------->91 x 127

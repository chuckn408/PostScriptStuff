# PostScriptStuff

Just a small collection of my postscript notes

--Postcript files in .ps
--files are run through GhostScript

https://ghostscript.com/releases/gsdnld.html

First reference site::
https://paulbourke.net/dataformats/postscript/

Some other useful Commands::

-The following are some other commonly used commands along with a brief description, again you should consult a reference manual for the entire set of commands. 	

-Draws an arc (including a circle). The arguments are xcenter, ycenter, radius, start angle, stop angle. The arc is drawn counterclockwise, the angles are in units of degrees.

-This is an example of an instruction that takes no arguments but leaves numbers on the stack, namely the coordinates of the current point.

-This sets the dash attribute of a line in terms of a mark-space array. Just as strings are denoted by round braces (), arrays are denoted by square braces []. For example the following command "[3 3] 0 setdash" would make any following lines have a 3 unit dash followed by a 3 unit space. The argument after the dash array is the offset for the start of the first dash.

-This specifies what the ends of a stroked line look like. It takes one argument which may be 0 (butt caps), 1 (round caps), or 2 (extended butt caps). The radius of round caps and the extension of the butt caps is determined by the line thickness. 

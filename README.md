# SolidCam-Mach3-Post
## A SolidCam postprocessor for Mach3, supporting 4x and 5x operations

Inspired by bogan - http://www.cnczone.com/forums/solidcam/255556-cnc.html

Setup: standard 3 axis mill. A axis rotary, along X.

##Current status :
 - 3 axis - considered working
 - 4 axis - works for both repositioning moves and 4x toolpaths
 - 5 axis - works. Problems with inversion seem to be fixed now !!!
 - Drill seems to work
 - Tapping seems to work
 - fhgdgfd
 
**This post is yet to produce code that has been run on a real machine ! Use at your own risk !**
 
##TODO :
 - Arc feeds may need work
 - 4x indexial use may need some more work to avoid unnecessary retracts to clearance
 - Canned cycles of any kind
 - Tool offsets and compensation
 - Along Y version
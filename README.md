# SolidCam-Mach3-Post
## A SolidCam postprocessor for Mach3, supporting 4x and 5x operations

Inspired by bogan - http://www.cnczone.com/forums/solidcam/255556-cnc.html

**This post is yet to produce code that has been run on a real machine ! Use at your own risk !**

Setup: standard 3 axis mill. A axis rotary, along X.

##Current status :
 - 3 axis - considered working
 - 4 axis - works for both repositioning moves and 4x toolpaths
 - 5 axis - works. Problems with inversion seem to be fixed now !!!
 - Drill seems to work
 - Tapping seems to work
 
##TODO :
 - Arc feeds may need work
 - 4x indexial use may need some more work to avoid unnecessary retracts to clearance
 - Canned cycles of any kind
 - Tool offsets and compensation
 - Along Y version

##Installation and usage notes :
 - PP install - Put the gpp and vmid files in `C:\Users\Public\Documents\SolidCAM\SolidCAM2015\Gpptool`
 - Usage in SolidCam - Select `Mach3_4X` for CNC-Machine
 - Mach3 setup
  * Config > General Config - tick `A-axis is angular`, set `IJ mode` to incremental, uncheck all in `Rotational`, possibly also check `G04 dwell in ms`
  * Config > Toolpath - Check `X-axis` for axis of rotation and enable `A-rotations`. `3d compass` also helps.

**Usage : Do set your CoorSyses so that the CS origin is in the pivot point (axis of rotation) and X is the axis around which the part revolves**
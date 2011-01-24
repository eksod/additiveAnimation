DISCLAIMER:
This software is provided 'as-is', without any express or implied warranty.  In no event will the authors be held liable for any damages arising from the use of this script.


INSTRUCTIONS:
This is a script for Autodesk Motionbuilder which creates an additive animation to be used on real-time engines, where the animation is to be "added" over others. 

For this you just need a scene with a single characterized character and it's control rig. This scene should contain an animation ploted on Take01 and the pose ploted on Take02, both with "Plot on all keys" active, plus an empty Take03. It work as:

Take 01 - Take 02 = Take 03

Where:

Take 01: is the animation itself.
Take 02: the animation to be subtracted (a walk pose for example)
Take 03: take where the result will be applied.

The length of the animation is taken from take01.


INSTALL:
There's no install, on Motionbuilder just go to Window/Python Editor. On the second button chose to open additiveAnimation.py from where you saved it. Then press Execute Active Work Area (fifth button, with the little arrow.)

Use the Gremlin example provided. It's a sample scene that comes with Motionbuilder with an example animation. Open, see what's on each take and run it to see the results. The script plots the animation, but I would recommend plotting it manually before running it anyway (for some reason, pyfbsdk's PlotAnimation() is not getting animation from non-characterized bones from other layers).


If you have any questions, ideas or feature requests please contact the author at:
'Eduardo Simioni' <eduardo.simioni@gmail.com>
http://www.eksod.com
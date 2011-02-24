DISCLAIMER:
This software is provided 'as-is', without any express or implied warranty.  In no event will the authors be held liable for any damages arising from the use of this script.


INSTRUCTIONS:
This is a script for Autodesk Motionbuilder which creates an additive animation to be used on real-time engines, where the animation is to be "added" over others. 

To run it you need a scene with a single character, preferably characterized but not necessarily. This scene should contain an animation ploted on Take01 and the pose (or base animation) ploted on Take02, plus an empty Take03. It work as:

Take 01 - Take 02 = Take 03

Where:

Take 01: is the animation itself.
Take 02: the animation to be subtracted (a walk pose for example)
Take 03: take where the result will be applied.

The length of the animation is taken from take01.

The animation on the game is most probably going to be added over the "bind/stance pose" of the character. If you don't have the joint/bones rotations zeroed out at the bind pose you need to add it to take03. This is done automatically with the script if there is a character by taking the bind pose used on the characterization process. This bind pose on Motionbuilder must be the same as on the game for the animation to work.


INSTALL:
There's no install, on Motionbuilder just go to Window/Python Editor. On the second button chose to open additiveAnimation.py from where you saved it. Then press Execute Active Work Area (fifth button, with the little arrow.)

Study the Gremlin example provided for a moment. It's a sample scene that comes with Motionbuilder with an example animation. Open, see what's on each take and run it to see the results. The script plots the animation, but I would recommend plotting it manually before running it anyway (for some reason, pyfbsdk's PlotAnimation() is not getting animation from non-characterized bones from other layers).


If you have any questions, ideas or feature requests please contact the author at:
'Eduardo Simioni' <eduardo.simioni@gmail.com>
http://www.eksod.com
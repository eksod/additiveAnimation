DISCLAIMER:
This software is provided 'as-is', without any express or implied warranty.  In no event will the authors be held liable for any damages arising from the use of this script.


INSTRUCTIONS:
This creates an additive animation to be used on real-time engines, where the animation is to be "added" over another playing animation. You shouldn't actually subtract one animation from the other, but a "pose" (on Take02) from the animation on Take01.

For this you need just a scene with a single characherized character and it's control rig. This scene should contain an animation ploted on Take01 and the pose ploted on Take02, both with "Plot on all keys" active, plus an empty or not Take03. It work as:

Take 01 - Take 02 = Take 03

Where:

Take 01: is the animation itself.
Take 02: the animation to be substracted (a walk pose for example)
Take 03: take where the result will be applied.

The length of the animation is taken from take01, take02.


INSTALL:
There's no install, on Motionbuilder just go to Window/Python Editor. On the second button chose to open additiveAnimation.py from where you saved it. Then press Execute Active Work Area (fifth button, with the little arrow.)


If you have any questions, ideas or feature requests please contact the author at:
'Eduardo Simioni' <eduardo.simioni@gmail.com>
http://www.eksod.com
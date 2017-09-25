.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

blendMode()
===========

Blends the pixels in the display window according to the defined mode.
There is a choice of the following modes to blend the source pixels (A)
with the ones of pixels already in the display window (B):

BLEND - linear interpolation of colours: C =
A*factor + B. This is the default blending mode.
ADD - sum of A and B
DARKEST - only the darkest colour succeeds: C =
min(A*factor, B).
LIGHTEST - only the lightest colour succeeds: C =
max(A*factor, B).
DIFFERENCE - subtract colors from underlying image.
EXCLUSION - similar to DIFFERENCE, but less
extreme.
MULTIPLY - multiply the colors, result will always be
darker.
SCREEN - opposite multiply, uses inverse values of the
colors.
REPLACE - the pixels entirely replace the others and
don't utilize alpha (transparency) values.
OVERLAY - mix of MULTIPLY and SCREEN
. Multiplies dark values, and screens light values.
HARD_LIGHT - SCREEN when greater than 50%
gray, MULTIPLY when lower.
SOFT_LIGHT - mix of DARKEST and
LIGHTEST. Works like OVERLAY, but not as harsh.

DODGE - lightens light tones and increases contrast,
ignores darks.
BURN - darker areas are applied, increasing contrast,
ignores lights.


**รูปแบบการใช้งาน**

blendMode ( mode )

**พารามิเตอร์**

- ``mode``  Constant: blend mode to set for canvas. either BLEND, DARKEST, LIGHTEST, DIFFERENCE, MULTIPLY, EXCLUSION, SCREEN, REPLACE, OVERLAY, HARD_LIGHT, SOFT_LIGHT, DODGE, BURN, ADD or NORMAL


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	blendMode(LIGHTEST);
	strokeWeight(30);
	stroke(80, 150, 255);
	line(25, 25, 75, 75);
	stroke(255, 50, 50);
	line(75, 25, 25, 75);

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	blendMode(MULTIPLY);
	strokeWeight(30);
	stroke(80, 150, 255);
	line(25, 25, 75, 75);
	stroke(255, 50, 50);
	line(75, 25, 25, 75);

	</script>

	<br><br>

.. toctree::


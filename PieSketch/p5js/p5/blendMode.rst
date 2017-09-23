.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

blendMode()
===========

Blends the pixels in the display window according to the defined mode.
There is a choice of the following modes to blend the source pixels (A)
with the ones of pixels already in the display window (B):
<ul>
<li><code>BLEND</code> - linear interpolation of colours: C =
A*factor + B. This is the default blending mode.</li>
<li><code>ADD</code> - sum of A and B</li>
<li><code>DARKEST</code> - only the darkest colour succeeds: C =
min(A*factor, B).</li>
<li><code>LIGHTEST</code> - only the lightest colour succeeds: C =
max(A*factor, B).</li>
<li><code>DIFFERENCE</code> - subtract colors from underlying image.</li>
<li><code>EXCLUSION</code> - similar to <code>DIFFERENCE</code>, but less
extreme.</li>
<li><code>MULTIPLY</code> - multiply the colors, result will always be
darker.</li>
<li><code>SCREEN</code> - opposite multiply, uses inverse values of the
colors.</li>
<li><code>REPLACE</code> - the pixels entirely replace the others and
don't utilize alpha (transparency) values.</li>
<li><code>OVERLAY</code> - mix of <code>MULTIPLY</code> and <code>SCREEN
</code>. Multiplies dark values, and screens light values.</li>
<li><code>HARD_LIGHT</code> - <code>SCREEN</code> when greater than 50%
gray, <code>MULTIPLY</code> when lower.</li>
<li><code>SOFT_LIGHT</code> - mix of <code>DARKEST</code> and
<code>LIGHTEST</code>. Works like <code>OVERLAY</code>, but not as harsh.
</li>
<li><code>DODGE</code> - lightens light tones and increases contrast,
ignores darks.</li>
<li><code>BURN</code> - darker areas are applied, increasing contrast,
ignores lights.</li>
</ul>

**รูปแบบการใช้งาน**

blendMode ( mode )

**พารามิเตอร์**

- ``mode``  : blend mode to set for canvas. either BLEND, DARKEST, LIGHTEST, DIFFERENCE, MULTIPLY, EXCLUSION, SCREEN, REPLACE, OVERLAY, HARD_LIGHT, SOFT_LIGHT, DODGE, BURN, ADD or NORMAL


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


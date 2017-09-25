.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

rotate()
========

Rotates a shape the amount specified by the angle parameter. This
function accounts for angleMode, so angles can be entered in either
RADIANS or DEGREES.

Objects are always rotated around their relative position to the
origin and positive numbers rotate objects in a clockwise direction.
Transformations apply to everything that happens after and subsequent
calls to the function accumulates the effect. For example, calling
rotate(HALF_PI) and then rotate(HALF_PI) is the same as rotate(PI).
All tranformations are reset when draw() begins again.

Technically, rotate() multiplies the current transformation matrix
by a rotation matrix. This function can be further controlled by
the push() and pop().

**รูปแบบการใช้งาน**

rotate ( angle, [axis] )

**พารามิเตอร์**

- ``angle``  Number: the angle of rotation, specified in radians or degrees, depending on current angleMode

- ``axis``  p5.Vector,Array: (in 3d) the axis to rotate around


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	translate(width/2, height/2);
	rotate(PI/3.0);
	rect(-26, -26, 52, 52);

	</script>

	<br><br>

.. toctree::


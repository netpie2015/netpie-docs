.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

shearX()
========

Shears a shape around the x-axis the amount specified by the angle
parameter. Angles should be specified in the current angleMode.
Objects are always sheared around their relative position to the origin
and positive numbers shear objects in a clockwise direction.

Transformations apply to everything that happens after and subsequent
calls to the function accumulates the effect. For example, calling
shearX(PI/2) and then shearX(PI/2) is the same as shearX(PI).
If shearX() is called within the draw(), the transformation is reset when
the loop begins again.

Technically, shearX() multiplies the current transformation matrix by a
rotation matrix. This function can be further controlled by the
push() and pop() functions.

**รูปแบบการใช้งาน**

shearX ( angle )

**พารามิเตอร์**

- ``angle``  : angle of shear specified in radians or degrees, depending on current angleMode


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	translate(width/4, height/4);
	shearX(PI/4.0);
	rect(0, 0, 30, 30);
	</script>

	<br><br>

.. toctree::


.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

magSq()
=======

Calculates the squared magnitude of the vector and returns the result
as a float (this is simply the equation <em>(x*x + y*y + z*z)</em>.)
Faster if the real length is not required in the
case of comparing vectors, etc.

**รูปแบบการใช้งาน**

magSq ( )

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	// Static method
	var v1 = createVector(6, 4, 2);
	print(v1.magSq()); // Prints "56"
	</script>

	<br><br>

.. toctree::


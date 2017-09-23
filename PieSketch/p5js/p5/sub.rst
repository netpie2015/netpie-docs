.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

sub()
=====

Subtracts x, y, and z components from a vector, subtracts one vector from
another, or subtracts two independent vectors. The version of the method
that subtracts two vectors is a static method and returns a p5.Vector, the
other acts directly on the vector. See the examples for more context.

**รูปแบบการใช้งาน**

sub ( x, [y], [z] )

**พารามิเตอร์**

- ``x``  : the x component of the vector or a p5.Vector or an Array

- ``y``  : the y component of the vector

- ``z``  : the z component of the vector


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var v = createVector(4, 5, 6);
	v.sub(1, 1, 1);
	// v's components are set to [3, 4, 5]
	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	// Static method
	var v1 = createVector(2, 3, 4);
	var v2 = createVector(1, 2, 3);
	
	var v3 = p5.Vector.sub(v1, v2);
	// v3 has components [1, 1, 1]
	</script>

	<br><br>

.. toctree::


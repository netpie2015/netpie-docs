.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

array()
=======

Return a representation of this vector as a float array. This is only
for temporary use. If used in any other fashion, the contents should be
copied by using the p5.Vector.copy() method to copy into your own
array.

**รูปแบบการใช้งาน**

array ( )

**ค่าที่ส่งออกมา**

- Array.<Number>: an Array with the 3 values


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	  var v = createVector(20,30);
	  print(v.array()); // Prints : Array [20, 30, 0]
	}

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var v = createVector(10.0, 20.0, 30.0);
	var f = v.array();
	print(f[0]); // Prints "10.0"
	print(f[1]); // Prints "20.0"
	print(f[2]); // Prints "30.0"

	</script>

	<br><br>

.. toctree::


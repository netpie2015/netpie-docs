.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

mag()
=====

Calculates the magnitude (length) of the vector and returns the result as
a float (this is simply the equation sqrt(x*x + y*y + z*z).)

**รูปแบบการใช้งาน**

mag ( )

**ค่าที่ส่งออกมา**

- Number: magnitude of the vector


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var v = createVector(20.0, 30.0, 40.0);
	var m = v.mag();
	print(m); // Prints "53.85164807134504"

	</script>

	<br><br>

.. toctree::


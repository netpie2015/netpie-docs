.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

noiseSeed()
===========

Sets the seed value for noise(). By default, noise()
produces different results each time the program is run. Set the
value parameter to a constant to return the same pseudo-random
numbers each time the software is run.

**รูปแบบการใช้งาน**

noiseSeed ( seed )

**พารามิเตอร์**

- ``seed``  Number: the seed value


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var xoff = 0.0;
	
	function setup() {
	  noiseSeed(99);
	  stroke(0, 10);
	}
	
	function draw() {
	  xoff = xoff + .01;
	  var n = noise(xoff) * width;
	  line(n, 0, n, height);
	}

	</script>

	<br><br>

.. toctree::


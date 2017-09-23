.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

randomSeed()
============

Sets the seed value for random().
By default, random() produces different results each time the program
is run. Set the seed parameter to a constant to return the same
pseudo-random numbers each time the software is run.

**รูปแบบการใช้งาน**

randomSeed ( seed )

**พารามิเตอร์**

- ``seed``  : the seed value


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	randomSeed(99);
	for (var i=0; i < 100; i++) {
	  var r = random(0, 255);
	  stroke(r);
	  line(i, 0, i, 100);
	}
	</script>

	<br><br>

.. toctree::


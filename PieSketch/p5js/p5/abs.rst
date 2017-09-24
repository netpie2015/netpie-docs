.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

abs()
=====

Calculates the absolute value (magnitude) of a number. Maps to Math.abs().
The absolute value of a number is always positive.

**รูปแบบการใช้งาน**

abs ( n )

**พารามิเตอร์**

- ``n``  Number: number to compute


**ค่าที่ส่งออกมา**

- Number: absolute value of given number


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	  var x = -3;
	  var y = abs(x);
	
	  print(x); // -3
	  print(y); // 3
	}


	</script>

	<br><br>

.. toctree::


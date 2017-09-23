.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

float()
=======

Converts a string to its floating point representation. The contents of a
string must resemble a number, or NaN (not a number) will be returned.
For example, float("1234.56") evaluates to 1234.56, but float("giraffe")
will return NaN.
When an array of values is passed in, then an array of floats of the same
length is returned.

**รูปแบบการใช้งาน**

float ( str )

**พารามิเตอร์**

- ``str``  : float string to parse


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var str = '20';
	var diameter = float(str);
	ellipse(width/2, height/2, diameter, diameter);
	</script>

	<br><br>

.. toctree::


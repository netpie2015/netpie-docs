.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

split()
=======

The split() function maps to String.split(), it breaks a String into
pieces using a character or string as the delimiter. The delim parameter
specifies the character or characters that mark the boundaries between
each piece. A String[] array is returned that contains each of the pieces.
The splitTokens() function works in a similar fashion, except that it
splits using a range of characters instead of a specific character or
sequence.

**รูปแบบการใช้งาน**

split ( value, delim )

**พารามิเตอร์**

- ``value``  String: the String to be split

- ``delim``  String: the String used to separate the data


**ค่าที่ส่งออกมา**

- Array.<String>: Array of Strings


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var names = "Pat,Xio,Alex"
	var splitString = split(names, ",");
	text(splitString[0], 5, 30);
	text(splitString[1], 5, 50);
	text(splitString[2], 5, 70);


	</script>

	<br><br>

.. toctree::


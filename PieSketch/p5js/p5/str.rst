.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

str()
=====

Converts a boolean, string or number to its string representation.
When an array of values is passed in, then an array of strings of the same
length is returned.

**รูปแบบการใช้งาน**

str ( n )

**พารามิเตอร์**

- ``n``  String,Boolean,Number,Array: value to parse


**ค่าที่ส่งออกมา**

- String: string representation of value


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	print(str("10"));  // "10"
	print(str(10.31)); // "10.31"
	print(str(-10));   // "-10"
	print(str(true));  // "true"
	print(str(false)); // "false"
	print(str([true, "10.3", 9.8])); // [ "true", "10.3", "9.8" ]

	</script>

	<br><br>

.. toctree::


.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

boolean()
=========

Converts a number or string to its boolean representation.
For a number, any non-zero value (positive or negative) evaluates to true,
while zero evaluates to false. For a string, the value "true" evaluates to
true, while any other value evaluates to false. When an array of number or
string values is passed in, then a array of booleans of the same length is
returned.

**รูปแบบการใช้งาน**

boolean ( n )

**พารามิเตอร์**

- ``n``  String,Boolean,Number,Array: value to parse


**ค่าที่ส่งออกมา**

- Boolean: boolean representation of value


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	print(boolean(0));               // false
	print(boolean(1));               // true
	print(boolean("true"));          // true
	print(boolean("abcd"));          // false
	print(boolean([0, 12, "true"])); // [false, true, false]

	</script>

	<br><br>

.. toctree::


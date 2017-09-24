.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

match()
=======

This function is used to apply a regular expression to a piece of text,
and return matching groups (elements found inside parentheses) as a
String array. If there are no matches, a null value will be returned.
If no groups are specified in the regular expression, but the sequence
matches, an array of length 1 (with the matched text as the first element
of the array) will be returned.

To use the function, first check to see if the result is null. If the
result is null, then the sequence did not match at all. If the sequence
did match, an array is returned.

If there are groups (specified by sets of parentheses) in the regular
expression, then the contents of each will be returned in the array.
Element [0] of a regular expression match returns the entire matching
string, and the match groups start at element [1] (the first group is [1],
the second [2], and so on).

**รูปแบบการใช้งาน**

match ( str, regexp )

**พารามิเตอร์**

- ``str``  String: the String to be searched

- ``regexp``  String: the regexp to be used for matching


**ค่าที่ส่งออกมา**

- Array.<String>: Array of Strings found


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var string = "Hello p5js*!"
	var regexp = "p5js\\*"
	var match = match(string, regexp);
	text(match, 5, 50);


	</script>

	<br><br>

.. toctree::


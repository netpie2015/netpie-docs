.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

splitTokens()
=============

The splitTokens() function splits a String at one or many character
delimiters or "tokens." The delim parameter specifies the character or
characters to be used as a boundary.

If no delim characters are specified, any whitespace character is used to
split. Whitespace characters include tab (\t), line feed (\n), carriage
return (\r), form feed (\f), and space.

**รูปแบบการใช้งาน**

splitTokens ( value, [delim] )

**พารามิเตอร์**

- ``value``  String: the String to be split

- ``delim``  String: list of individual Strings that will be used as separators


**ค่าที่ส่งออกมา**

- Array.<String>: Array of Strings


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	  var myStr = "Mango, Banana, Lime";
	  var myStrArr = splitTokens(myStr, ",");
	
	  print(myStrArr); // prints : ["Mango"," Banana"," Lime"]
	}


	</script>

	<br><br>

.. toctree::


.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

shorten()
=========

Decreases an array by one element and returns the shortened array,
maps to Array.pop().

**รูปแบบการใช้งาน**

shorten ( list )

**พารามิเตอร์**

- ``list``  Array: Array to shorten


**ค่าที่ส่งออกมา**

- Array: shortened Array


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	  var myArray = new Array("A", "B", "C");
	  print(myArray); // ["A","B","C"]
	
	  var newArray = shorten(myArray);
	  print(myArray); // ["A","B","C"]
	  print(newArray); // ["A","B"]
	}

	</script>

	<br><br>

.. toctree::


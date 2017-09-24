.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

append()
========

Adds a value to the end of an array. Extends the length of
the array by one. Maps to Array.push().

**รูปแบบการใช้งาน**

append ( array, value )

**พารามิเตอร์**

- ``array``  Array: Array to append

- ``value``  any: to be added to the Array


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	
	var myArray = new Array("Mango", "Apple", "Papaya")
	print(myArray) // ["Mango", "Apple", "Papaya"]
	
	append(myArray, "Peach")
	print(myArray) // ["Mango", "Apple", "Papaya", "Peach"]
	
	}


	</script>

	<br><br>

.. toctree::


.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

reverse()
=========

Reverses the order of an array, maps to Array.reverse()

**รูปแบบการใช้งาน**

reverse ( list )

**พารามิเตอร์**

- ``list``  Array: Array to reverse


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	  var myArray = new Array("A", "B", "C");
	  print(myArray); // ["A","B","C"]
	
	  reverse(myArray);
	  print(myArray); // ["C","B","A"]
	}

	</script>

	<br><br>

.. toctree::


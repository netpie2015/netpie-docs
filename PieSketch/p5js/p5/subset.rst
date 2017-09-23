.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

subset()
========

Extracts an array of elements from an existing array. The list parameter
defines the array from which the elements will be copied, and the start
and count parameters specify which elements to extract. If no count is
given, elements will be extracted from the start to the end of the array.
When specifying the start, remember that the first array element is 0.
This function does not change the source array.

**รูปแบบการใช้งาน**

subset ( list, start, [count] )

**พารามิเตอร์**

- ``list``  : Array to extract from

- ``start``  : position to begin

- ``count``  : number of values to extract


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	  var myArray = new Array(1,2,3,4,5);
	  print(myArray); // [1,2,3,4,5]
	
	  var sub1 = subset(myArray, 0, 3);
	  var sub2 = subset(myArray, 2, 2);
	  print(sub1); // [1,2,3]
	  print(sub2); // [3,4]
	}
	</script>

	<br><br>

.. toctree::


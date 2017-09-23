.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

splice()
========

Inserts a value or an array of values into an existing array. The first
parameter specifies the initial array to be modified, and the second
parameter defines the data to be inserted. The third parameter is an index
value which specifies the array position from which to insert data.
(Remember that array index numbering starts at zero, so the first position
is 0, the second position is 1, and so on.)

**รูปแบบการใช้งาน**

splice ( list, value, position )

**พารามิเตอร์**

- ``list``  : Array to splice into

- ``value``  : value to be spliced in

- ``position``  : in the array from which to insert data


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	  var myArray = new Array(0,1,2,3,4);
	  var insArray = new Array("A","B","C");
	  print(myArray); // [0,1,2,3,4]
	  print(insArray); // ["A","B","C"]
	
	  splice(myArray, insArray, 3);
	  print(myArray); // [0,1,2,"A","B","C",3,4]
	}
	</script>

	<br><br>

.. toctree::


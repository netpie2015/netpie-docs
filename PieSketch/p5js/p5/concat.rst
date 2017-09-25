.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

concat()
========

Concatenates two arrays, maps to Array.concat(). Does not modify the
input arrays.

**รูปแบบการใช้งาน**

concat ( a, b )

**พารามิเตอร์**

- ``a``  Array: first Array to concatenate

- ``b``  Array: second Array to concatenate


**ค่าที่ส่งออกมา**

- Array: concatenated array


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	  var arr1 = new Array("A", "B", "C");
	  var arr2 = new Array( 1 ,  2 ,  3 );
	
	  print(arr1); // ["A","B","C"]
	  print(arr2); // [1,2,3]
	
	  var arr3 = concat(arr1, arr2);
	
	  print(arr1); // ["A","B","C"]
	  print(arr2); // [1,2,3]
	  print(arr3); // ["A","B","C",1,2,3]
	
	}

	</script>

	<br><br>

.. toctree::


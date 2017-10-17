.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

concat()
========

เชื่อมต่ออาร์เรย์สองชุดเข้ากับ Array.concat () ไม่แก้ไขอาร์เรย์ของอินพุต

.. Concatenates two arrays, maps to Array.concat(). Does not modify the
.. input arrays.

**รูปแบบการใช้งาน**

concat ( a, b )

**พารามิเตอร์**

- ``a``  Array: อาร์เรย์แรกที่ต่อกัน

- ``b``  Array: อาร์เรย์ที่สองให้ต่อกัน

.. ``a``  Array: first Array to concatenate
.. ``b``  Array: second Array to concatenate

**ค่าที่ส่งออกมา**

- Array: อาร์เรย์ที่ต่อกัน

.. Array: concatenated array

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

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.

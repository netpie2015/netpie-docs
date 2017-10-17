.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

shorten()
=========

ลดอาร์เรย์โดยองค์ประกอบหนึ่งและส่งกลับค่าอาร์เรย์ที่สั้นลงไปยัง Array.pop ()

.. Decreases an array by one element and returns the shortened array,
.. maps to Array.pop().

**รูปแบบการใช้งาน**

shorten ( list )

**พารามิเตอร์**

- ``list``  Array: อาร์เรย์ย่อ

.. ``list``  Array: Array to shorten

**ค่าที่ส่งออกมา**

- Array: ย่ออาร์เรย์

.. Array: shortened Array

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

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.

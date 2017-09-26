.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

subset()
========

แยกอาร์เรย์ของอิลิเมนต์ออกจากอาร์เรย์ที่มีอยู่ พารามิเตอร์รายการกำหนดอาร์เรย์ที่จะคัดลอกองค์ประกอบและพารามิเตอร์เริ่มต้นและการนับระบุองค์ประกอบที่จะแยก ถ้าไม่มีการนับจำนวนองค์ประกอบจะถูกแยกออกจากจุดเริ่มต้นจนถึงจุดสิ้นสุดของอาร์เรย์ เมื่อระบุการเริ่มต้นโปรดจำไว้ว่าองค์ประกอบอาร์เรย์แรกคือ 0 ฟังก์ชันนี้จะไม่เปลี่ยนอาร์เรย์ของแหล่งข้อมูล

.. Extracts an array of elements from an existing array. The list parameter
.. defines the array from which the elements will be copied, and the start
.. and count parameters specify which elements to extract. If no count is
.. given, elements will be extracted from the start to the end of the array.
.. When specifying the start, remember that the first array element is 0.
.. This function does not change the source array.

**รูปแบบการใช้งาน**

subset ( list, start, [count] )

**พารามิเตอร์**

- ``list``  Array: อาร์เรย์ที่สกัดจาก

- ``start``  Number: ตำแหน่งที่จะเริ่มต้น

- ``count``  Number: จำนวนค่าที่จะแยก

.. ``list``  Array: Array to extract from
.. ``start``  Number: position to begin
.. ``count``  Number: number of values to extract

**ค่าที่ส่งออกมา**

- Array: อาร์เรย์ขององค์ประกอบที่แยกออกมา

.. Array: Array of extracted elements

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

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

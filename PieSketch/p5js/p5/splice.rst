.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

splice()
========

แทรกค่าหรืออาร์เรย์ของค่าลงในอาร์เรย์ที่มีอยู่ พารามิเตอร์แรกกำหนดอาร์เรย์เริ่มต้นที่จะแก้ไขและพารามิเตอร์ที่สองกำหนดข้อมูลที่จะแทรก พารามิเตอร์ที่สามคือค่าดัชนีที่ระบุตำแหน่งอาร์เรย์ที่จะแทรกข้อมูล (จำหมายเลขดัชนีอาเรย์เริ่มต้นที่ศูนย์ดังนั้นอันดับแรกคือ 0 ตำแหน่งที่สองคือ 1 และอื่น ๆ )

.. Inserts a value or an array of values into an existing array. The first
.. parameter specifies the initial array to be modified, and the second
.. parameter defines the data to be inserted. The third parameter is an index
.. value which specifies the array position from which to insert data.
.. (Remember that array index numbering starts at zero, so the first position
.. is 0, the second position is 1, and so on.)

**รูปแบบการใช้งาน**

splice ( list, value, position )

**พารามิเตอร์**

- ``list``  Array: อาร์เรย์ที่จะเข้าร่วม

- ``value``  any: ค่าที่จะเชื่อมต่อเข้า

- ``position``  Number: ในอาร์เรย์ที่จะแทรกข้อมูล

.. ``list``  Array: Array to splice into
.. ``value``  any: value to be spliced in
.. ``position``  Number: in the array from which to insert data

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

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

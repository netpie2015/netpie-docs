.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

ambientMaterial()
=================

วัสดุล้อมรอบสำหรับเรขาคณิตด้วยสีที่กำหนด คุณสามารถดูวัสดุที่เป็นไปได้ทั้งหมดใน ตัวอย่าง นี้

.. Ambient material for geometry with a given color. You can view all
.. possible materials in this
.. example.

**รูปแบบการใช้งาน**

ambientMaterial ( v1, [v2], [v3], [a] )

**พารามิเตอร์**

- ``v1``  Number,Array,String,p5.Color: ค่าสีเทาค่าสีแดงหรือสี (ขึ้นอยู่กับโหมดสีปัจจุบัน) หรืออาร์เรย์สีหรือสตริงสี CSS

- ``v2``  Number: ตัวเลือก: สีเขียวหรือความอิ่มตัวของสี

- ``v3``  Number: ตัวเลือก: สีน้ำเงินหรือความสว่าง

- ``a``  Number: ตัวเลือก: ความทึบ

.. ``v1``  Number,Array,String,p5.Color: gray value, red or hue value (depending on the current color mode), or color Array, or CSS color string
.. ``v2``  Number: optional: green or saturation value
.. ``v3``  Number: optional: blue or brightness value
.. ``a``  Number: optional: opacity

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup(){
	  createCanvas(100, 100, WEBGL);
	}
	function draw(){
	 background(0);
	 ambientLight(100);
	 pointLight(250, 250, 250, 100, 100, 0);
	 ambientMaterial(250);
	 sphere(50);
	}

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.

.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

fill()
======

เติมวัสดุพื้นฐานสำหรับเรขาคณิตด้วยสีที่กำหนด

.. Basic fill material for geometry with a given color
**รูปแบบการใช้งาน**

fill ( v1, [v2], [v3], [a] )

**พารามิเตอร์**

- ``v1``  Number,Array,String,p5.Color: ค่าสีเทาค่าสีแดงหรือสี (ขึ้นอยู่กับโหมดสีปัจจุบัน) หรืออาร์เรย์สีหรือสตริงสี CSS

- ``v2``  Number: ตัวเลือก: สีเขียวหรือความอิ่มตัวของสี

- ``v3``  Number: ตัวเลือก: สีน้ำเงินหรือความสว่าง

- ``a``  Number: ตัวเลือก: ความทึบ

.. ``v1``  Number,Array,String,p5.Color: gray value,
red or hue value (depending on the current color mode),
or color Array, or CSS color string
.. ``v2``  Number: optional: green or saturation value
.. ``v3``  Number: optional: blue or brightness value
.. ``a``  Number: optional: opacity

**ค่าที่ส่งออกมา**

- p5: วัตถุ p5

.. p5: the p5 object

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup(){
	  createCanvas(200, 200, WEBGL);
	}
	
	function draw(){
	 background(0);
	 noStroke();
	 fill(100, 100, 240);
	 rotateX(frameCount * 0.01);
	 rotateY(frameCount * 0.01);
	 box(75, 75, 75);
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

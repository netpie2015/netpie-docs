.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

hue()
=====

แยกค่าสีออกจากอาร์เรย์สีหรือพิกเซล ฮิวอยู่ใน HSB และ HSL ฟังก์ชั่นนี้จะส่งกลับสี HSB ตามปกติเมื่อให้มาพร้อมกับวัตถุสี HSB (หรือเมื่อมาพร้อมกับอาร์เรย์พิกเซลในขณะที่โหมดสีเป็น HSB) แต่จะเป็นค่าเริ่มต้นของสี HSL-normalized (ค่าจะแตกต่างกันถ้าการตั้งค่าสีสูงสุดสำหรับแต่ละระบบแตกต่างกัน)

.. Extracts the hue value from a color or pixel array.
.. Hue exists in both HSB and HSL. This function will return the
.. HSB-normalized hue when supplied with an HSB color object (or when supplied
.. with a pixel array while the color mode is HSB), but will default to the
.. HSL-normalized hue otherwise. (The values will only be different if the
.. maximum hue setting for each system is different.)

**รูปแบบการใช้งาน**

hue ( color )

**พารามิเตอร์**

- ``color``  p5.Color,Array: p5.Color object หรือ pixel array

.. ``color``  p5.Color,Array: p5.Color object or pixel array

**ค่าที่ส่งออกมา**

- Number: สีสัน

.. Number: the hue

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	noStroke();
	colorMode(HSB, 255);
	c = color(0, 126, 255);
	fill(c);
	rect(15, 20, 35, 60);
	value = hue(c);  // Sets 'value' to "0"
	fill(value);
	rect(50, 20, 35, 60);

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

saturation()
============

แยกค่าความอิ่มตัวจากอาร์เรย์สีหรือพิกเซล ความอิ่มตัวของสีจะแตกต่างกันไปใน HSB และ HSL ฟังก์ชั่นนี้จะส่งกลับค่าความอิ่มตัวของ HSB เมื่อมีวัตถุสี HSB (หรือเมื่อมาพร้อมกับพิกเซลในขณะที่โหมดสีเป็น HSB) แต่จะมีความอิ่มตัวของ HSL ตามค่าดีฟอลต์

.. Extracts the saturation value from a color or pixel array.
.. Saturation is scaled differently in HSB and HSL. This function will return
.. the HSB saturation when supplied with an HSB color object (or when supplied
.. with a pixel array while the color mode is HSB), but will default to the
.. HSL saturation otherwise.

**รูปแบบการใช้งาน**

saturation ( color )

**พารามิเตอร์**

- ``color``  p5.Color,Array: p5.Color object หรือ pixel array

.. ``color``  p5.Color,Array: p5.Color object or pixel array

**ค่าที่ส่งออกมา**

- Number: ค่าความอิ่มตัว

.. Number: the saturation value

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	noStroke();
	colorMode(HSB, 255);
	c = color(0, 126, 255);
	fill(c);
	rect(15, 20, 35, 60);
	value = saturation(c);  // Sets 'value' to 126
	fill(value);
	rect(50, 20, 35, 60);

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.

.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

lerpColor()
===========

ผสมสีสองสีเพื่อหาสีที่สามระหว่างที่อยู่ พารามิเตอร์ amt คือจำนวนที่จะสอดแทรกระหว่างสองค่าซึ่ง 0.0 เท่ากับสีแรกซึ่ง 0.1 ใกล้เคียงกับสีแรก 0.5 อยู่กึ่งกลางระหว่างเป็นต้นจำนวนเงินที่ต่ำกว่า 0 จะถือว่าเท่ากับ 0. ในทำนองเดียวกันจำนวนเงินที่กล่าวมาข้างต้น 1 จะถูก จำกัด ไว้ที่ 1 ซึ่งแตกต่างจากพฤติกรรมของ lerp () แต่จำเป็นเนื่องจากมิฉะนั้นตัวเลขนอกช่วงจะทำให้เกิดสีแปลก ๆ และไม่คาดคิด 
วิธีที่สี interpolated ขึ้นอยู่กับโหมดสีปัจจุบัน

.. Blends two colors to find a third color somewhere between them. The amt
.. parameter is the amount to interpolate between the two values where 0.0
.. equal to the first color, 0.1 is very near the first color, 0.5 is halfway
.. in between, etc. An amount below 0 will be treated as 0. Likewise, amounts
.. above 1 will be capped at 1. This is different from the behavior of lerp(),
.. but necessary because otherwise numbers outside the range will produce
.. strange and unexpected colors.
.. 
.. The way that colours are interpolated depends on the current color mode.
**รูปแบบการใช้งาน**

lerpColor ( c1, c2, amt )

**พารามิเตอร์**

- ``c1``  p5.Color: interpolate จากสีนี้

- ``c2``  p5.Color: interpolate กับสีนี้

- ``amt``  Number: หมายเลขระหว่าง 0 ถึง 1

.. ``c1``  p5.Color: interpolate from this color
.. ``c2``  p5.Color: interpolate to this color
.. ``amt``  Number: number between 0 and 1

**ค่าที่ส่งออกมา**

- p5.Color: สี interpolated

.. p5.Color: interpolated color

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	colorMode(RGB);
	stroke(255);
	background(51);
	from = color(218, 165, 32);
	to = color(72, 61, 139);
	colorMode(RGB);  // Try changing to HSB.
	interA = lerpColor(from, to, .33);
	interB = lerpColor(from, to, .66);
	fill(from);
	rect(10, 20, 20, 60);
	fill(interA);
	rect(30, 20, 20, 60);
	fill(interB);
	rect(50, 20, 20, 60);
	fill(to);
	rect(70, 20, 20, 60);

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

blendMode()
===========

ผสมผสานพิกเซลในหน้าต่างแสดงผลตามโหมดที่กำหนด มีโหมดต่อไปนี้ให้เลือกผสมผสานพิกเซลต้นฉบับ (A) กับพิกเซลที่มีอยู่ในหน้าต่างแสดงผล (B):  BLEND - การแก้ไขเชิงเส้นของสี: C = A * factor + B นี่เป็นโหมดการผสมเริ่มต้น  ADD - ผลรวมของ A และ B  DARKEST - เฉพาะสีที่มืดที่สุดเท่านั้นที่ประสบความสำเร็จ: C = min (A * factor, B)  LIGHTEST - เฉพาะสีที่เบาที่สุดเท่านั้นที่ประสบความสำเร็จ: C = max (A * factor, B)  DIFFERENCE - ลบสีจากภาพต้นแบบ  EXCLUSION - คล้ายคลึงกับ DIFFERENCE แต่ไม่รุนแรงมากนัก  MULTIPLY - คูณสีผลจะเป็นสีเข้มเสมอ  SCREEN - ตรงข้ามคูณใช้ค่าผกผันของสี  REPLACE - พิกเซลทั้งหมดแทนที่ผู้อื่นและไม่ใช้ค่า alpha (โปร่งใส)  OVERLAY - การผสมผสานของ MULTIPLY และ SCREEN คูณค่าความสว่างและค่าแสงของหน้าจอ  HARD_LIGHT - SCREEN เมื่อสีเทามากกว่า 50% MULTIPLY เมื่อลดลง  SOFT_LIGHT - ผสมผสานระหว่าง DARKEST และ LIGHTEST ที่สุด ทำงานได้เหมือน OVERLAY แต่ไม่รุนแรงมากนัก  DODGE - ลดแสงและเพิ่มความคมชัดและไม่สนใจ Darks  BURN - ใช้พื้นที่เข้มขึ้นเพิ่มความคมชัดไม่สนใจไฟ 

.. Blends the pixels in the display window according to the defined mode.
.. There is a choice of the following modes to blend the source pixels (A)
.. with the ones of pixels already in the display window (B):
.. 
.. BLEND - linear interpolation of colours: C =
.. A*factor + B. This is the default blending mode.
.. ADD - sum of A and B
.. DARKEST - only the darkest colour succeeds: C =
.. min(A*factor, B).
.. LIGHTEST - only the lightest colour succeeds: C =
.. max(A*factor, B).
.. DIFFERENCE - subtract colors from underlying image.
.. EXCLUSION - similar to DIFFERENCE, but less
.. extreme.
.. MULTIPLY - multiply the colors, result will always be
.. darker.
.. SCREEN - opposite multiply, uses inverse values of the
.. colors.
.. REPLACE - the pixels entirely replace the others and
.. don't utilize alpha (transparency) values.
.. OVERLAY - mix of MULTIPLY and SCREEN
.. . Multiplies dark values, and screens light values.
.. HARD_LIGHT - SCREEN when greater than 50%
.. gray, MULTIPLY when lower.
.. SOFT_LIGHT - mix of DARKEST and
.. LIGHTEST. Works like OVERLAY, but not as harsh.
.. 
.. DODGE - lightens light tones and increases contrast,
.. ignores darks.
.. BURN - darker areas are applied, increasing contrast,
.. ignores lights.
.. 

**รูปแบบการใช้งาน**

blendMode ( mode )

**พารามิเตอร์**

- ``mode``  Constant: ผสมผสานการตั้งค่าสำหรับผ้าใบ ทั้ง BLEND, DARKEST, LIGHTEST, DIFFERENCE, MULTIPLY, EXCLUSION, SCREEN, REPLACE, OVERLAY, HARD_LIGHT, SOFT_LIGHT, DODGE, BURN, ADD หรือ NORMAL

.. ``mode``  Constant: blend mode to set for canvas. either BLEND, DARKEST, LIGHTEST, DIFFERENCE, MULTIPLY, EXCLUSION, SCREEN, REPLACE, OVERLAY, HARD_LIGHT, SOFT_LIGHT, DODGE, BURN, ADD or NORMAL

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	blendMode(LIGHTEST);
	strokeWeight(30);
	stroke(80, 150, 255);
	line(25, 25, 75, 75);
	stroke(255, 50, 50);
	line(75, 25, 25, 75);

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	blendMode(MULTIPLY);
	strokeWeight(30);
	stroke(80, 150, 255);
	line(25, 25, 75, 75);
	stroke(255, 50, 50);
	line(75, 25, 25, 75);

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.

.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

endContour()
============

ใช้ฟังก์ชัน beginContour () และ endContour () เพื่อสร้างรูปร่างเชิงลบภายในรูปร่างเช่นตรงกลางของตัวอักษร &#39;O&#39; beginContour () เริ่มบันทึกจุดสำหรับรูปร่างและ endContour () หยุดการบันทึก จุดที่กำหนดรูปร่างเชิงลบต้อง &quot;ลม&quot; ไปในทิศทางตรงกันข้ามกับรูปทรงภายนอก วาดจุดแรกสำหรับคำสั่งภายนอกตามเข็มนาฬิกาแล้วสำหรับรูปร่างภายในให้วาดรูปร่างของยอดในทวนเข็มนาฬิกา 
ฟังก์ชันเหล่านี้สามารถใช้งานได้ภายในคู่สัญญา beginShape () / endShape () เท่านั้นและการแปลงเช่น translate (), rotate () และ scale () ไม่ทำงานภายในคู่ beginContour () / endContour () นอกจากนี้ยังไม่สามารถใช้รูปทรงอื่น ๆ เช่นวงรี () หรือ rect () ภายในได้

.. Use the beginContour() and endContour() functions to create negative
.. shapes within shapes such as the center of the letter 'O'. beginContour()
.. begins recording vertices for the shape and endContour() stops recording.
.. The vertices that define a negative shape must "wind" in the opposite
.. direction from the exterior shape. First draw vertices for the exterior
.. clockwise order, then for internal shapes, draw vertices
.. shape in counter-clockwise.
.. 
.. These functions can only be used within a beginShape()/endShape() pair and
.. transformations such as translate(), rotate(), and scale() do not work
.. within a beginContour()/endContour() pair. It is also not possible to use
.. other shapes, such as ellipse() or rect() within.

**รูปแบบการใช้งาน**

endContour ( )

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	translate(50, 50);
	stroke(255, 0, 0);
	beginShape();
	// Exterior part of shape, clockwise winding
	vertex(-40, -40);
	vertex(40, -40);
	vertex(40, 40);
	vertex(-40, 40);
	// Interior part of shape, counter-clockwise winding
	beginContour();
	vertex(-20, -20);
	vertex(-20, 20);
	vertex(20, 20);
	vertex(20, -20);
	endContour();
	endShape(CLOSE);

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

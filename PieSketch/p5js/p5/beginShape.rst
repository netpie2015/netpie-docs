.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

beginShape()
============

การใช้ฟังก์ชัน beginShape () และ endShape () ช่วยในการสร้างฟอร์มที่ซับซ้อนมากขึ้น beginShape () เริ่มบันทึกจุดสำหรับรูปร่างและ endShape () หยุดการบันทึก ค่าของพารามิเตอร์ชนิดระบุชนิดของรูปร่างที่จะสร้างจากจุดยอดที่ให้ไว้ โดยไม่มีการระบุโหมดรูปร่างอาจเป็นรูปหลายเหลี่ยมที่ไม่สม่ำเสมอ 
พารามิเตอร์ที่ใช้ได้สำหรับ beginShape () คือ POINTS, LINES, TRIANGLES, TRIANGLE_FAN, TRIANGLE_STRIP, QUADS และ QUAD_STRIP หลังจากเรียกใช้ฟังก์ชัน beginShape () แล้วชุดคำสั่ง vertex () ต้องปฏิบัติตาม หากต้องการหยุดการวาดรูปให้โทร endShape () แต่ละรูปร่างจะถูกร่างด้วยสีของจังหวะในปัจจุบันและเต็มไปด้วยสีเติม 
การแปลงเช่น translate (), rotate () และ scale () ไม่ทำงานภายใน beginShape () นอกจากนี้ยังไม่สามารถใช้รูปร่างอื่น ๆ ได้เช่นวงรี () หรือ rect () ภายใน beginShape ()

.. Using the beginShape() and endShape() functions allow creating more
.. complex forms. beginShape() begins recording vertices for a shape and
.. endShape() stops recording. The value of the kind parameter tells it which
.. types of shapes to create from the provided vertices. With no mode
.. specified, the shape can be any irregular polygon.
.. 
.. The parameters available for beginShape() are POINTS, LINES, TRIANGLES,
.. TRIANGLE_FAN, TRIANGLE_STRIP, QUADS, and QUAD_STRIP. After calling the
.. beginShape() function, a series of vertex() commands must follow. To stop
.. drawing the shape, call endShape(). Each shape will be outlined with the
.. current stroke color and filled with the fill color.
.. 
.. Transformations such as translate(), rotate(), and scale() do not work
.. within beginShape(). It is also not possible to use other shapes, such as
.. ellipse() or rect() within beginShape().
**รูปแบบการใช้งาน**

beginShape ( [kind] )

**พารามิเตอร์**

- ``kind``  Constant: ทั้ง POINTS, LINES, TRIANGLES, TRIANGLE_FAN TRIANGLE_STRIP, QUADS หรือ QUAD_STRIP

.. ``kind``  Constant: either POINTS, LINES, TRIANGLES, TRIANGLE_FAN
                               TRIANGLE_STRIP, QUADS, or QUAD_STRIP

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	beginShape();
	vertex(30, 20);
	vertex(85, 20);
	vertex(85, 75);
	vertex(30, 75);
	endShape(CLOSE);

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	// currently not working
	beginShape(POINTS);
	vertex(30, 20);
	vertex(85, 20);
	vertex(85, 75);
	vertex(30, 75);
	endShape();

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	beginShape(LINES);
	vertex(30, 20);
	vertex(85, 20);
	vertex(85, 75);
	vertex(30, 75);
	endShape();

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	noFill();
	beginShape();
	vertex(30, 20);
	vertex(85, 20);
	vertex(85, 75);
	vertex(30, 75);
	endShape();

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	noFill();
	beginShape();
	vertex(30, 20);
	vertex(85, 20);
	vertex(85, 75);
	vertex(30, 75);
	endShape(CLOSE);

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	beginShape(TRIANGLES);
	vertex(30, 75);
	vertex(40, 20);
	vertex(50, 75);
	vertex(60, 20);
	vertex(70, 75);
	vertex(80, 20);
	endShape();

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	beginShape(TRIANGLE_STRIP);
	vertex(30, 75);
	vertex(40, 20);
	vertex(50, 75);
	vertex(60, 20);
	vertex(70, 75);
	vertex(80, 20);
	vertex(90, 75);
	endShape();

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	beginShape(TRIANGLE_FAN);
	vertex(57.5, 50);
	vertex(57.5, 15);
	vertex(92, 50);
	vertex(57.5, 85);
	vertex(22, 50);
	vertex(57.5, 15);
	endShape();

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	beginShape(QUADS);
	vertex(30, 20);
	vertex(30, 75);
	vertex(50, 75);
	vertex(50, 20);
	vertex(65, 20);
	vertex(65, 75);
	vertex(85, 75);
	vertex(85, 20);
	endShape();

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	beginShape(QUAD_STRIP);
	vertex(30, 20);
	vertex(30, 75);
	vertex(50, 20);
	vertex(50, 75);
	vertex(65, 20);
	vertex(65, 75);
	vertex(85, 20);
	vertex(85, 75);
	endShape();

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	beginShape();
	vertex(20, 20);
	vertex(40, 20);
	vertex(40, 40);
	vertex(60, 40);
	vertex(60, 60);
	vertex(20, 60);
	endShape(CLOSE);

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

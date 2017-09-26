.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

redraw()
========

ดำเนินการรหัสภายใน draw () หนึ่งครั้ง ฟังก์ชันนี้ช่วยให้โปรแกรมสามารถปรับปรุงหน้าต่างแสดงผลได้เฉพาะเมื่อจำเป็นเท่านั้นเช่นเมื่อเหตุการณ์ที่ลงทะเบียนโดย mousePressed () หรือ keyPressed () เกิดขึ้น 
ในการจัดโครงสร้างโปรแกรมจะทำให้เรียกซ้ำการวาดภาพ () ซ้ำภายในเหตุการณ์เช่น mousePressed () เนื่องจากการวาดใหม่ () ไม่ได้เรียกใช้ draw () ทันที (มีการตั้งค่าสถานะที่ระบุว่าจำเป็นต้องอัปเดตเท่านั้น) 
ฟังก์ชัน redraw () ไม่ทำงานอย่างถูกต้องเมื่อเรียกภายใน draw () หากต้องการเปิด / ปิดการใช้งานภาพเคลื่อนไหวให้ใช้ loop () และ noLoop () 
นอกจากนี้คุณสามารถกำหนดจำนวนของภาพวาดต่อการเรียกใช้เมธอด เพียงเพิ่มจำนวนเต็มเป็นพารามิเตอร์เดียวสำหรับจำนวนภาพวาด

.. Executes the code within draw() one time. This functions allows the
.. program to update the display window only when necessary, for example
.. when an event registered by mousePressed() or keyPressed() occurs.
.. 
.. In structuring a program, it only makes sense to call redraw() within
.. events such as mousePressed(). This is because redraw() does not run
.. draw() immediately (it only sets a flag that indicates an update is
.. needed).
.. 
.. The redraw() function does not work properly when called inside draw().
.. To enable/disable animations, use loop() and noLoop().
.. 
.. In addition you can set the number of redraws per method call. Just
.. add an integer as single parameter for the number of redraws.

**รูปแบบการใช้งาน**

redraw ( [n] )

**พารามิเตอร์**

- ``n``  Integer: วาดซ้ำสำหรับ n-times ค่าดีฟอลต์คือ 1

.. ``n``  Integer: Redraw for n-times. The default value is 1.

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var x = 0;
	
	function setup() {
	  createCanvas(100, 100);
	  noLoop();
	}
	
	function draw() {
	  background(204);
	  line(x, 0, x, height);
	}
	
	function mousePressed() {
	  x += 1;
	  redraw();
	}
	var x = 0;
	
	function setup() {
	  createCanvas(100, 100);
	  noLoop();
	}
	
	function draw() {
	  background(204);
	  x += 1;
	  line(x, 0, x, height);
	}
	
	function mousePressed() {
	  redraw(5);
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

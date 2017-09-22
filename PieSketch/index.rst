.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

PieSketch
=========

PieSketch เป็นเครื่องมือช่วยพัฒนา application แบบ web-based ที่ทีมพัฒนา NETPIE ตั้งใจออกแบบขึ้นมา สำหรับผู้ใช้มือใหม่ และมือสมัครเล่น ที่เพิ่งหัดเขียนโปรแกรม ใช้เป็นสนามในการสร้างสรรและแบ่งปันผลงาน Pie Sketch ได้รวมโมดูลต่างๆ ที่รองรับการทำงานกับ ภาพ, เสียง, กราฟฟิคเคลื่อนไหว รวมไปถึงความสามารถในการเชื่อมต่อ NETPIE platform สำหรับออกแบบ IOT application ที่สื่อสารกันบนหน้าจอได้อย่างรวดเร็วและสนุกสนาน

การใช้งาน
--------
บริการของ PieSketch เข้าถึงได้ทาง https://sketch.netpie.io

.. image:: _static/screenshot-01.png

เริ่มต้นกับ sketch แรก
--------------------

โค้ดของ PieSketch มีพื้นฐานอยู่บน `p5js <https://p5js.org>`_. โครงสร้างประกอบด้วย 2 ฟังก์ชั่นหลัก ได้แก่ setup() ซึ่งจะถูกเรียกครั้งเดียวตอนแรกที่โปรแกรมถูกรัน และ draw() ที่จะถูกเรียกซ้ำๆไปตลอด โค้ดตัวอย่าง จะเป็นการวาดรูปวงกลม เส้นผ่านศูนย์กลาง 80 จุดศูนย์กลางที่ตำแหน่ง (50,50)

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {

	}

	function draw() {
	  ellipse(50, 50, 80, 80);
	}
	</script>

ชุดคำสั่งใน PieSketch
-------------------

.. toctree::
   :maxdepth: 2

   p5js toolset  : เครื่องมือช่วยออกแบบโปรแกรมอย่างง่าย <p5/index>
   Microgear : เชื่อมต่อ IOT กับ NETPIE <microgear/index>


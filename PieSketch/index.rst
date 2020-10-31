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

- `p5js <p5js/index.html>`_  เป็นเครื่องมือช่วยพัฒนาโปรแกรมบน HTML5 ในรูปแบบที่ไม่ซับซ้อน ประกอบด้วย ฟังก์ชั่นเกี่ยวกับ การแสดงผลแสงสีบนจอภาพ การควบคุมอุปกรณ์อย่างเมาส์และคีย์บอร์ด รวมไปถึงฟังก์ชั่นช่วยเหลือด้านการคำนวณทางคณิตศาสตร์ รวมไปถึงฟังก์ชั่นเสริม ที่ช่วยให้เราสื่อสารกับ HTML5 object ที่อยู่นอกเหนือจาก canvas เช่น ปุ่มกด, วิดีโอ, เว็บแคม

- `NETPIE <netpie/index.html>`_ เป็นชุดคำสั่ง สำหรับพัฒนาโปรแกรมที่เชื่อมต่อกับ NETPIE platform เราสามารถสร้าง sketch ที่สื่อสารกับส่วนประกอบอื่นของ NETPIE เช่น device, dashboard, data feed, mobile push notification หรือแม่แต่ sketch สื่อสารกันเองเป็นกลุ่ม

.. toctree::
	:hidden:

	p5js <p5js/index>
	NETPIE <netpie/index>

ตัวอย่างโค้ด PieSketch
--------------------


- `p5js และ NETPIE <examples/index.html>`_

.. toctree::
	:hidden:

	p5js และ NETPIE <examples/index>



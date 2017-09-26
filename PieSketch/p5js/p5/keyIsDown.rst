.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

keyIsDown()
===========

ฟังก์ชัน keyIsDown () จะตรวจสอบว่าคีย์อยู่ในขณะนี้หรือไม่เช่นกดปุ่ม สามารถใช้งานได้ถ้าคุณมีวัตถุเคลื่อนที่และคุณต้องการให้คีย์หลายตัวสามารถส่งผลต่อพฤติกรรมของตัวเองได้พร้อม ๆ กันเช่นการย้ายสไปรต์ตามแนวทแยงมุม คุณสามารถใส่หมายเลขใด ๆ แทน keyCode ของคีย์หรือใช้ชื่อคีย์โคดตัวแปรใดก็ได้ ที่นี่

.. The keyIsDown() function checks if the key is currently down, i.e. pressed.
.. It can be used if you have an object that moves, and you want several keys
.. to be able to affect its behaviour simultaneously, such as moving a
.. sprite diagonally. You can put in any number representing the keyCode of
.. the key, or use any of the variable keyCode names listed
.. here.

**รูปแบบการใช้งาน**

keyIsDown ( code )

**พารามิเตอร์**

- ``code``  Number: กุญแจสำคัญในการตรวจสอบ

.. ``code``  Number: The key to check for.

**ค่าที่ส่งออกมา**

- Boolean: ไม่ว่าคีย์จะลงหรือไม่

.. Boolean: whether key is down or not

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var x = 100;
	var y = 100;
	
	function setup() {
	  createCanvas(512, 512);
	}
	
	function draw() {
	  if (keyIsDown(LEFT_ARROW))
	    x-=5;
	
	  if (keyIsDown(RIGHT_ARROW))
	    x+=5;
	
	  if (keyIsDown(UP_ARROW))
	    y-=5;
	
	  if (keyIsDown(DOWN_ARROW))
	    y+=5;
	
	  clear();
	  fill(255, 0, 0);
	  ellipse(x, y, 50, 50);
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

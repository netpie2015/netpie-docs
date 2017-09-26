.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

randomGaussian()
================

ส่งกลับค่าจำนวนสุ่มที่เหมาะสมกับการแจกแจงแบบเกาส์หรือแบบปกติ ในทางทฤษฎีไม่มีค่าต่ำสุดหรือสูงสุดที่ randomGaussian () อาจส่งคืน ค่อนข้างมีเพียงความเป็นไปได้ต่ำมากที่ค่าที่ห่างไกลจากค่าเฉลี่ยจะถูกส่งกลับ และความเป็นไปได้สูงที่ตัวเลขที่ใกล้เคียงกับค่าเฉลี่ยจะถูกส่งกลับ 
ใช้อาร์กิวเมนต์ 0, 1 หรือ 2 
ถ้าไม่มี args ให้ค่าเฉลี่ยของ 0 และส่วนเบี่ยงเบนมาตรฐานเท่ากับ 1 
ถ้า arg หนึ่งอาร์กิวเมนต์นี้เป็นค่าเฉลี่ย (ส่วนเบี่ยงเบนมาตรฐานคือ 1) 
ถ้า args สองตัวแรกหมายถึงส่วนที่สองคือส่วนเบี่ยงเบนมาตรฐาน

.. Returns a random number fitting a Gaussian, or
.. normal, distribution. There is theoretically no minimum or maximum
.. value that randomGaussian() might return. Rather, there is
.. just a very low probability that values far from the mean will be
.. returned; and a higher probability that numbers near the mean will
.. be returned.
.. 
.. Takes either 0, 1 or 2 arguments.
.. If no args, returns a mean of 0 and standard deviation of 1.
.. If one arg, that arg is the mean (standard deviation is 1).
.. If two args, first is mean, second is standard deviation.

**รูปแบบการใช้งาน**

randomGaussian ( mean, sd )

**พารามิเตอร์**

- ``mean``  Number: ความหมาย

- ``sd``  Number: ค่าเบี่ยงเบนมาตรฐาน

.. ``mean``  Number: the mean
.. ``sd``  Number: the standard deviation

**ค่าที่ส่งออกมา**

- Number: จำนวนสุ่ม

.. Number: the random number

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	for (var y = 0; y < 100; y++) {
	 var x = randomGaussian(50,15);
	 line(50, y, x, y);
	}

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var distribution = new Array(360);
	
	function setup() {
	 createCanvas(100, 100);
	 for (var i = 0; i < distribution.length; i++) {
	   distribution[i] = floor(randomGaussian(0,15));
	 }
	}
	
	function draw() {
	 background(204);
	
	 translate(width/2, width/2);
	
	 for (var i = 0; i < distribution.length; i++) {
	   rotate(TWO_PI/distribution.length);
	   stroke(0);
	   var dist = abs(distribution[i]);
	   line(0, 0, dist, 0);
	 }
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

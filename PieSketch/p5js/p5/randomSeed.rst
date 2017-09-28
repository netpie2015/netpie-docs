.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

randomSeed()
============

ตั้งค่าเมล็ดสำหรับ random () โดยค่าเริ่มต้น random () จะให้ผลลัพธ์ที่แตกต่างกันในแต่ละครั้งที่มีการเรียกใช้โปรแกรม ตั้งค่าพารามิเตอร์ seed เป็นค่าคงที่เพื่อให้ตัวเลข pseudo-random เดียวกันทุกครั้งที่มีการเรียกใช้ซอฟต์แวร์

.. Sets the seed value for random().
.. By default, random() produces different results each time the program
.. is run. Set the seed parameter to a constant to return the same
.. pseudo-random numbers each time the software is run.

**รูปแบบการใช้งาน**

randomSeed ( seed )

**พารามิเตอร์**

- ``seed``  Number: ค่าเมล็ด

.. ``seed``  Number: the seed value

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	randomSeed(99);
	for (var i=0; i < 100; i++) {
	  var r = random(0, 255);
	  stroke(r);
	  line(i, 0, i, 100);
	}

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.

.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

random()
========

ส่งคืนจำนวนจุดลอยตัวแบบสุ่ม ใช้อาร์กิวเมนต์ 0, 1 หรือ 2 ถ้าไม่ได้รับอาร์กิวเมนต์ให้ส่งคืนตัวเลขสุ่มตั้งแต่ 0 ถึง (แต่ไม่รวม) 1 ถ้าอาร์กิวเมนต์หนึ่งได้รับและเป็นตัวเลขให้ส่งกลับตัวเลขสุ่มจาก 0 ถึง (แต่ไม่รวม) จำนวน หากอาร์กิวเมนต์หนึ่งได้รับและเป็นอาร์เรย์ให้ส่งค่าองค์ประกอบแบบสุ่มจากอาร์เรย์นั้น ถ้าอาร์กิวเมนต์สองรายการได้รับให้ส่งกลับตัวเลขสุ่มจากอาร์กิวเมนต์แรกถึง (แต่ไม่รวม) อาร์กิวเมนต์ที่สอง

.. Return a random floating-point number.
.. Takes either 0, 1 or 2 arguments.
.. If no argument is given, returns a random number from 0
.. up to (but not including) 1.
.. If one argument is given and it is a number, returns a random number from 0
.. up to (but not including) the number.
.. If one argument is given and it is an array, returns a random element from
.. that array.
.. If two arguments are given, returns a random number from the
.. first argument up to (but not including) the second argument.

**รูปแบบการใช้งาน**

random ( [min], [max] )

**พารามิเตอร์**

- ``min``  Number: ขอบเขตล่าง (รวม)

- ``max``  Number: ขอบเขตบน (พิเศษ)

.. ``min``  Number: the lower bound (inclusive)
.. ``max``  Number: the upper bound (exclusive)

**ค่าที่ส่งออกมา**

- Number: จำนวนสุ่ม

.. Number: the random number

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	for (var i = 0; i < 100; i++) {
	  var r = random(50);
	  stroke(r*5);
	  line(50, i, 50+r, i);
	}

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	for (var i = 0; i < 100; i++) {
	  var r = random(-50, 50);
	  line(50,i,50+r,i);
	}

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	// Get a random element from an array using the random(Array) syntax
	var words = [ "apple", "bear", "cat", "dog" ];
	var word = random(words);  // select random word
	text(word,10,50);  // draw the word

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.

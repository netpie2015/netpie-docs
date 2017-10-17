.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

heading()
=========

คำนวณมุมของการหมุนสำหรับเวกเตอร์นี้ (เฉพาะเวกเตอร์ 2D)

.. Calculate the angle of rotation for this vector (only 2D vectors)

**รูปแบบการใช้งาน**

heading ( )

**ค่าที่ส่งออกมา**

- Number: มุมของการหมุน

.. Number: the angle of rotation

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	  var v1 = createVector(30,50);
	  print(v1.heading()); // 1.0303768265243125
	
	  var v1 = createVector(40,50);
	  print(v1.heading()); // 0.8960553845713439
	
	  var v1 = createVector(30,70);
	  print(v1.heading()); // 1.1659045405098132
	}

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.

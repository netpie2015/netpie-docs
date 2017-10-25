.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

strokeJoin()
============

กำหนดลักษณะของข้อต่อที่เชื่อมต่อส่วนของสาย ข้อต่อเหล่านี้มีทั้ง mitered, beveled หรือกลมและระบุด้วยพารามิเตอร์ที่เกี่ยวข้อง MITER, BEVEL และ ROUND ข้อต่อเริ่มต้นคือ MITER

.. Sets the style of the joints which connect line segments. These joints are either mitered, beveled, or rounded and specified with the corresponding parameters MITER, BEVEL, and ROUND. The default joint is MITER.

**รูปแบบการใช้งาน**

strokeJoin(join)

**พารามิเตอร์**

- ``join``  ค่าคงที่: MITER, BEVEL และ ROUND

.. - ``join``  Constant: either MITER, BEVEL, ROUND

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	noFill();
    strokeWeight(10.0);
    strokeJoin(MITER);
    beginShape();
    vertex(35, 20);
    vertex(65, 50);
    vertex(35, 80);
    endShape();
	</script>

	<br><br>

    <script type="text/p5" data-autoplay data-hide-sourcecode>
	noFill();
    strokeWeight(10.0);
    strokeJoin(BEVEL);
    beginShape();
    vertex(35, 20);
    vertex(65, 50);
    vertex(35, 80);
    endShape();
	</script>

	<br><br>

    <script type="text/p5" data-autoplay data-hide-sourcecode>
	noFill();
    strokeWeight(10.0);
    strokeJoin(ROUND);
    beginShape();
    vertex(35, 20);
    vertex(65, 50);
    vertex(35, 80);
    endShape();
	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.

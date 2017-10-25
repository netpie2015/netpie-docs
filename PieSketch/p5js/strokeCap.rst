.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

strokeCap()
===========

ตั้งค่าสไตล์สำหรับการแสดงผลส่วนท้ายบรรทัด ปลายทั้งสองยกกำลังสองขยายหรือโค้งมนซึ่งแต่ละอันจะระบุด้วยพารามิเตอร์ที่สอดคล้องกัน ได้แก่ SQUARE PROJECT และ ROUND ฝาครอบเริ่มต้นคือ ROUND

.. Sets the style for rendering line endings. These ends are either squared, extended, or rounded, each of which specified with the corresponding parameters: SQUARE, PROJECT, and ROUND. The default cap is ROUND.

**รูปแบบการใช้งาน**

strokeCap(cap)

**พารามิเตอร์**

- ``cap``  ค่าคงที่: SQUARE, PROJECT หรือ ROUND

.. - ``cap``  Constant: either SQUARE, PROJECT, or ROUND

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	strokeWeight(12.0);
    strokeCap(ROUND);
    line(20, 30, 80, 30);
    strokeCap(SQUARE);
    line(20, 50, 80, 50);
    strokeCap(PROJECT);
    line(20, 70, 80, 70);
	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.

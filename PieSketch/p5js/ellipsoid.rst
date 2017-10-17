.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

ellipsoid()
===========

วาดรูปทรงรีกับรัศมีที่กำหนด

.. Draw an ellipsoid with given radius

**รูปแบบการใช้งาน**

ellipsoid ( radiusx, radiusy, radiusz, [detailX], [detailY] )

**พารามิเตอร์**

- ``radiusx``  Number: xradius ของวงกลม

- ``radiusy``  Number: yradius ของวงกลม

- ``radiusz``  Number: zradius ของวงกลม

- ``detailX``  Number: ไม่จำเป็น: จำนวนกลุ่มส่วนที่มากขึ้นค่าเริ่มต้นของรูปทรงเรขาคณิตเรียบขึ้นคือ 24 หลีกเลี่ยงตัวเลขรายละเอียดข้างต้น 150 อาจทำให้เบราเซอร์ขัดข้อง

- ``detailY``  Number: ไม่จำเป็น: จำนวนกลุ่มส่วนที่มากขึ้นจะมีค่าเริ่มต้นของรูปทรงเรขาคณิตที่ราบรื่นขึ้น 16. หลีกเลี่ยงจำนวนรายละเอียดข้างต้น 150 อาจทำให้เบราเซอร์ขัดข้อง

.. ``radiusx``  Number: xradius of circle
.. ``radiusy``  Number: yradius of circle
.. ``radiusz``  Number: zradius of circle
.. ``detailX``  Number: optional: number of segments, the more segments the smoother geometry default is 24. Avoid detail number above 150, it may crash the browser.
.. ``detailY``  Number: optional: number of segments, the more segments the smoother geometry default is 16. Avoid detail number above 150, it may crash the browser.

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	// draw an ellipsoid with radius 20, 30 and 40.
	function setup(){
	  createCanvas(100, 100, WEBGL);
	}
	
	function draw(){
	  background(200);
	  ellipsoid(20, 30, 40);
	}

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.

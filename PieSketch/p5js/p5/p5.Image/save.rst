.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

save()
======

บันทึกภาพลงในไฟล์และบังคับให้เบราว์เซอร์ดาวน์โหลด ยอมรับสตริงที่สองสำหรับชื่อไฟล์และนามสกุลไฟล์รองรับ png (ค่าเริ่มต้น) และ jpg

.. Saves the image to a file and force the browser to download it.
.. Accepts two strings for filename and file extension
.. Supports png (default) and jpg.
**รูปแบบการใช้งาน**

save ( filename, extension )

**พารามิเตอร์**

- ``filename``  String: ให้ชื่อไฟล์ของคุณ

- ``extension``  String: &#39;png&#39; หรือ &#39;jpg&#39;

.. ``filename``  String: give your file a name
.. ``extension``  String: 'png' or 'jpg'

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var photo;
	
	function preload() {
	  photo = loadImage("assets/rockies.jpg");
	}
	
	function draw() {
	  image(photo, 0, 0);
	}
	
	function keyTyped() {
	  if (key == 's') {
	    photo.save("photo", "png");
	  }
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

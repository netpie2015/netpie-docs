.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

getURL()
========

ได้รับ URL ปัจจุบัน

.. Gets the current URL.
**รูปแบบการใช้งาน**

getURL ( )

**ค่าที่ส่งออกมา**

- String: URL

.. String: url

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var url;
	var x = 100;
	
	function setup() {
	  fill(0);
	  noStroke();
	  url = getURL();
	}
	
	function draw() {
	  background(200);
	  text(url, x, height/2);
	  x--;
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

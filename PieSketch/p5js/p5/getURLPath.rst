.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

getURLPath()
============

รับเส้นทาง URL ปัจจุบันเป็นอาร์เรย์

.. Gets the current URL path as an array.
**รูปแบบการใช้งาน**

getURLPath ( )

**ค่าที่ส่งออกมา**

- Array.<String>: ส่วนประกอบเส้นทาง

.. Array.<String>: path components

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	  var urlPath = getURLPath();
	  for (var i=0; i&lt;urlPath.length; i++) {
	    text(urlPath[i], 10, i*20+20);
	  }
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

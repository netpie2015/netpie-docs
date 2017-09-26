.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

getURLParams()
==============

รับ params URL ปัจจุบันเป็น Object

.. Gets the current URL params as an Object.

**รูปแบบการใช้งาน**

getURLParams ( )

**ค่าที่ส่งออกมา**

- Object: URL params

.. Object: URL params

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	// Example: http://p5js.org?year=2014&month=May&day=15
	
	function setup() {
	  var params = getURLParams();
	  text(params.day, 10, 20);
	  text(params.month, 10, 40);
	  text(params.year, 10, 60);
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

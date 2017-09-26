.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

maxKey()
========

ส่งคืนคีย์ที่สูงที่สุด

.. Return the highest key.
**รูปแบบการใช้งาน**

maxKey ( )

**ค่าที่ส่งออกมา**

- Number: 

.. Number: 

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	  var myDictionary = createNumberDict({ 2 : 4, 4 : 6, 1.2 : 3});
	  var highestKey = myDictionary.maxKey(); // value is 4
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

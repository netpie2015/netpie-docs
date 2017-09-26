.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

minKey()
========

ส่งคืนคีย์ที่ต่ำที่สุด

.. Return the lowest key.
**รูปแบบการใช้งาน**

minKey ( )

**ค่าที่ส่งออกมา**

- Number: 

.. Number: 

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	  var myDictionary = createNumberDict({2 : 4, 4 : 6, 1.2 : 3});
	  var lowestKey = myDictionary.minKey(); // value is 1.2
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

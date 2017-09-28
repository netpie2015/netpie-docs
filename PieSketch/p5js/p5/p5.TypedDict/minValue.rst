.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

minValue()
==========

ส่งคืนค่าต่ำสุด

.. Return the lowest value.

**รูปแบบการใช้งาน**

minValue ( )

**ค่าที่ส่งออกมา**

- Number: 

.. Number: 

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	  var myDictionary = createNumberDict({2 : -10, 4 : 0.65, 1.2 : 3});
	  var lowestValue = myDictionary.minValue(); // value is -10
	}

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.

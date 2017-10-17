.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

maxValue()
==========

ส่งคืนค่าสูงสุด

.. Return the highest value.

**รูปแบบการใช้งาน**

maxValue ( )

**ค่าที่ส่งออกมา**

- Number: 

.. Number: 

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	  var myDictionary = createNumberDict({2 : -10, 4 : 0.65, 1.2 : 3});
	  var highestValue = myDictionary.maxValue(); // value is 3
	}

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.

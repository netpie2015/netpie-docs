.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

size()
======

แสดงจำนวนคู่คีย์ - ค่าที่อยู่ในออบเจ็กต์ Dictionary

.. Returns the number of key-value pairs currently in Dictionary object

**รูปแบบการใช้งาน**

size ( )

**ค่าที่ส่งออกมา**

- Number: จำนวนคู่คีย์ - ค่าในออบเจ็กต์ Dictionary

.. Number: the number of key-value pairs in Dictionary object

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	function setup() {
	  var myDictionary = createNumberDict(1, 10);
	  myDictionary.create(2, 20);
	  myDictionary.create(3, 30);
	  var amt = myDictionary.size(); // value of amt is 3
	}
	

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

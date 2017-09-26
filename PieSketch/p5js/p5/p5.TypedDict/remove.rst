.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

remove()
========

ลบคู่คีย์ - ค่าในพจนานุกรม

.. Removes a key-value pair in the Dictionary
**รูปแบบการใช้งาน**

remove ( key )

**พารามิเตอร์**

- ``key``  Number,String: สำหรับคู่ที่จะลบ

.. ``key``  Number,String: for the pair to remove

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	function setup() {
	  var myDictionary = createStringDict('p5', 'js');
	  myDictionary.create('happy', 'coding');
	  myDictionary.print()
	  // above logs "key: p5 - value: js, key: happy - value: coding" to console
	  myDictionary.remove('p5');
	  myDictionary.print();
	  // above logs "key: happy value: coding" to console
	}
	

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

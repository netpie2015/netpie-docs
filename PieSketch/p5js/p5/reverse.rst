.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

reverse()
=========

เปลี่ยนลำดับของอาร์เรย์กลับไปที่ Array.reverse ()

.. Reverses the order of an array, maps to Array.reverse()

**รูปแบบการใช้งาน**

reverse ( list )

**พารามิเตอร์**

- ``list``  Array: อาร์เรย์ย้อนกลับ

.. ``list``  Array: Array to reverse

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	  var myArray = new Array("A", "B", "C");
	  print(myArray); // ["A","B","C"]
	
	  reverse(myArray);
	  print(myArray); // ["C","B","A"]
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

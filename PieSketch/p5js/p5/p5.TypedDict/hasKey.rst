.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

hasKey()
========

ส่งกลับค่าจริงถ้าคีย์มีอยู่ในพจนานุกรมมิฉะนั้นจะส่งกลับค่าเท็จ

.. Returns true if key exists in Dictionary
.. otherwise returns false
**รูปแบบการใช้งาน**

hasKey ( key )

**พารามิเตอร์**

- ``key``  Number,String: ที่คุณต้องการเข้าถึง

.. ``key``  Number,String: that you want to access

**ค่าที่ส่งออกมา**

- Boolean: ว่าคีย์นั้นมีอยู่ในพจนานุกรมหรือไม่

.. Boolean: whether that key exists in Dictionary

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	function setup() {
	  var myDictionary = createStringDict('p5', 'js');
	  print(myDictionary.hasKey('p5')); // logs true to console
	}
	

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

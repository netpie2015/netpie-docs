.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

get()
=====

ส่งคืนค่าที่จัดเก็บไว้ในคีย์ที่ให้มา

.. Returns value stored at supplied key.
**รูปแบบการใช้งาน**

get ( key )

**พารามิเตอร์**

- ``key``  Number,String: ที่คุณต้องการเข้าถึง

.. ``key``  Number,String: that you want to access

**ค่าที่ส่งออกมา**

- Number,String: ค่าที่เก็บไว้ที่คีย์นั้น

.. Number,String: the value stored at that key

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	function setup() {
	  var myDictionary = createStringDict('p5', 'js');
	  var myValue = myDictionary.get('p5');
	  print(myValue === 'js'); // logs true to console
	}
	

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

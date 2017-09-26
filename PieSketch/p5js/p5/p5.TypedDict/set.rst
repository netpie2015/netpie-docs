.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

set()
=====

เปลี่ยนค่าของคีย์หากอยู่ในนั้นมีอยู่แล้วในในพจนานุกรมทำให้คู่คีย์ - ค่าใหม่

.. Changes the value of key if in it already exists in
.. in the Dictionary otherwise makes a new key-value pair

**รูปแบบการใช้งาน**

set ( key, value )

**พารามิเตอร์**

- ``key``  Number,String: 

- ``value``  Number,String: 

.. ``key``  Number,String: 
.. ``value``  Number,String: 

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	function setup() {
	  var myDictionary = createStringDict('p5', 'js');
	  myDictionary.set('p5', 'JS');
	  myDictionary.print()
	  // above logs "key: p5 - value: JS" to console
	}
	

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

div()
=====

หารค่าที่เก็บไว้ในคีย์หนึ่ง ๆ ผลหารจะถูกเก็บไว้ในตำแหน่งนั้นในพจนานุกรม

.. Divide a value stored at a certain key
.. The quotient is stored in that location in the Dictionary.
**รูปแบบการใช้งาน**

div ( Key, Amount )

**พารามิเตอร์**

- ``Key``  Number: สำหรับค่าที่คุณต้องการแบ่ง

- ``Amount``  Number: เพื่อหารค่าด้วย

.. ``Key``  Number: for value you wish to divide
.. ``Amount``  Number: to divide the value by

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	  var myDictionary = createNumberDict(2, 8);
	  myDictionary.div(2, 2);
	  console.log(myDictionary.get(2)); // logs 4 to console.
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

sub()
=====

ลบค่าที่จัดเก็บไว้ที่กุญแจหนึ่ง ๆ ความแตกต่างจะถูกเก็บไว้ในตำแหน่งนั้นในพจนานุกรม

.. Subtract from a value stored at a certain key
.. The difference is stored in that location in the Dictionary.

**รูปแบบการใช้งาน**

sub ( Key, Amount )

**พารามิเตอร์**

- ``Key``  Number: สำหรับค่าที่คุณต้องการลบ

- ``Amount``  Number: เพื่อลบออกจากค่า

.. ``Key``  Number: for value you wish to subtract from
.. ``Amount``  Number: to subtract from the value

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	  var myDictionary = createNumberDict(2, 5);
	  myDictionary.sub(2, 2);
	  console.log(myDictionary.get(2)); // logs 3 to console.
	}

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.

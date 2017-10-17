.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

add()
=====

จำนวนที่เก็บอยู่ในตำแหน่งนั้นในพจนานุกรม

.. Add to a value stored at a certain key
.. The sum is stored in that location in the Dictionary.

**รูปแบบการใช้งาน**

add ( Key, Amount )

**พารามิเตอร์**

- ``Key``  Number: สำหรับค่าที่คุณต้องการเพิ่ม

- ``Amount``  Number: เพื่อเพิ่มมูลค่า

.. ``Key``  Number: for value you wish to add to
.. ``Amount``  Number: to add to the value

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	  var myDictionary = createNumberDict(2, 5);
	  myDictionary.add(2, 2);
	  console.log(myDictionary.get(2)); // logs 7 to console.
	}

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.

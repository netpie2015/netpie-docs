.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

join()
======

รวมอาร์เรย์ของสตริงเข้าไว้ในสตริงเดียวแต่ละคั่นด้วยตัวอักษรที่ใช้สำหรับพารามิเตอร์คั่น เมื่อต้องการรวมอาร์เรย์ของ ints หรือ floats จำเป็นต้องแปลงเป็นสตริงโดยใช้ nf () หรือ nfs () ก่อน

.. Combines an array of Strings into one String, each separated by the
.. character(s) used for the separator parameter. To join arrays of ints or
.. floats, it's necessary to first convert them to Strings using nf() or
.. nfs().
**รูปแบบการใช้งาน**

join ( list, separator )

**พารามิเตอร์**

- ``list``  Array: อาร์เรย์ของสตริงที่จะรวม

- ``separator``  String: สตริงที่จะวางระหว่างแต่ละรายการ

.. ``list``  Array: array of Strings to be joined
.. ``separator``  String: String to be placed between each item

**ค่าที่ส่งออกมา**

- String: เข้าร่วม String

.. String: joined String

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var array = ["Hello", "world!"]
	var separator = " "
	var message = join(array, separator);
	text(message, 5, 50);

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

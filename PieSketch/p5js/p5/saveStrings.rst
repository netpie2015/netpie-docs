.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

saveStrings()
=============

เขียนอาร์เรย์ของสตริงในไฟล์ข้อความหนึ่งบรรทัดต่อสตริง กระบวนการบันทึกไฟล์และตำแหน่งของไฟล์ที่บันทึกไว้จะแตกต่างกันไปในแต่ละเว็บเบราเซอร์

.. Writes an array of Strings to a text file, one line per String.
..  The file saving process and location of the saved file will
..  vary between web browsers.
**รูปแบบการใช้งาน**

saveStrings ( list, filename )

**พารามิเตอร์**

- ``list``  Array: อาร์เรย์สตริงที่จะเขียน

- ``filename``  String: ชื่อไฟล์สำหรับเอาต์พุต

.. ``list``  Array: string array to be written
.. ``filename``  String: filename for output

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	 var words = 'apple bear cat dog';
	
	 // .split() outputs an Array
	 var list = split(words, ' ');
	
	 // To save the file, un-comment next line and click 'run'
	 // saveStrings(list, 'nouns.txt');
	
	 // Saves the following to a file called 'nouns.txt':
	 //
	 // apple
	 // bear
	 // cat
	 // dog
	 

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

splitTokens()
=============

ฟังก์ชัน splitTokens () แยกสตริงที่ตัวคั่นอักขระหนึ่งหรือหลายอักขระหรือ &quot;โทเค็น&quot; พารามิเตอร์ delim ระบุอักขระหรืออักขระที่จะใช้เป็นขอบเขต 
หากไม่มีการระบุอักขระ delim จะใช้อักขระ whitespace ใด ๆ ในการแบ่ง อักขระเว้นวรรค ได้แก่ แท็บ (\ t), ฟีดบรรทัด (\ n) การส่งคืน (\ r) ฟีดฟอร์ม (\ f) และช่องว่าง

.. The splitTokens() function splits a String at one or many character
.. delimiters or "tokens." The delim parameter specifies the character or
.. characters to be used as a boundary.
.. 
.. If no delim characters are specified, any whitespace character is used to
.. split. Whitespace characters include tab (\t), line feed (\n), carriage
.. return (\r), form feed (\f), and space.
**รูปแบบการใช้งาน**

splitTokens ( value, [delim] )

**พารามิเตอร์**

- ``value``  String: สายที่จะแยก

- ``delim``  String: รายการสตริงแต่ละตัวที่จะใช้เป็นตัวคั่น

.. ``value``  String: the String to be split
.. ``delim``  String: list of individual Strings that will be used as
                         separators

**ค่าที่ส่งออกมา**

- Array.<String>: อาร์เรย์ของสตริง

.. Array.<String>: Array of Strings

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	  var myStr = "Mango, Banana, Lime";
	  var myStrArr = splitTokens(myStr, ",");
	
	  print(myStrArr); // prints : ["Mango"," Banana"," Lime"]
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

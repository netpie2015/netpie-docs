.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

match()
=======

ฟังก์ชันนี้ใช้เพื่อใช้นิพจน์ทั่วไปกับข้อความและส่งคืนกลุ่มการจับคู่ (องค์ประกอบที่พบในวงเล็บ) เป็นอาร์เรย์สตริง ถ้าไม่มีการจับคู่ค่าที่เป็นค่า null จะถูกส่งกลับ หากไม่มีการระบุกลุ่มในนิพจน์ทั่วไป แต่ลำดับจะตรงกันอาร์เรย์ความยาว 1 (พร้อมข้อความที่ตรงกันเป็นองค์ประกอบแรกของอาร์เรย์) จะถูกส่งคืน 
เมื่อต้องการใช้ฟังก์ชันก่อนอื่นให้ตรวจดูว่าผลลัพธ์เป็นโมฆะหรือไม่ ถ้าผลลัพธ์เป็นโมฆะลำดับจะไม่ตรงกันเลย ถ้าลำดับไม่ตรงกันอาร์เรย์จะถูกส่งกลับ 
หากมีกลุ่ม (ระบุโดยวงเล็บ) ในนิพจน์ทั่วไปเนื้อหาของแต่ละรายการจะถูกส่งกลับในอาร์เรย์ Element [0] ของการจับคู่นิพจน์ทั่วไปจะส่งกลับสตริงที่ตรงกันทั้งหมดและกลุ่มการจับคู่เริ่มต้นที่องค์ประกอบ [1] (กลุ่มแรกคือ [1], สอง [2] และอื่น ๆ )

.. This function is used to apply a regular expression to a piece of text,
.. and return matching groups (elements found inside parentheses) as a
.. String array. If there are no matches, a null value will be returned.
.. If no groups are specified in the regular expression, but the sequence
.. matches, an array of length 1 (with the matched text as the first element
.. of the array) will be returned.
.. 
.. To use the function, first check to see if the result is null. If the
.. result is null, then the sequence did not match at all. If the sequence
.. did match, an array is returned.
.. 
.. If there are groups (specified by sets of parentheses) in the regular
.. expression, then the contents of each will be returned in the array.
.. Element [0] of a regular expression match returns the entire matching
.. string, and the match groups start at element [1] (the first group is [1],
.. the second [2], and so on).
**รูปแบบการใช้งาน**

match ( str, regexp )

**พารามิเตอร์**

- ``str``  String: สตริงที่จะค้นหา

- ``regexp``  String: regexp ที่จะใช้สำหรับการจับคู่

.. ``str``  String: the String to be searched
.. ``regexp``  String: the regexp to be used for matching

**ค่าที่ส่งออกมา**

- Array.<String>: พบอาร์เรย์ของ Strings

.. Array.<String>: Array of Strings found

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var string = "Hello p5js*!"
	var regexp = "p5js\\*"
	var match = match(string, regexp);
	text(match, 5, 50);

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

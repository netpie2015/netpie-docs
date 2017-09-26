.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

matchAll()
==========

ฟังก์ชันนี้ใช้เพื่อใช้นิพจน์ทั่วไปกับข้อความและส่งกลับรายการกลุ่มการจับคู่ (องค์ประกอบที่พบในวงเล็บ) เป็นอาร์เรย์สตริงแบบสองมิติ ถ้าไม่มีการจับคู่ค่าที่เป็นค่า null จะถูกส่งกลับ หากไม่มีการระบุกลุ่มในนิพจน์ทั่วไป แต่ลำดับตรงกับอาร์เรย์สองมิติจะถูกส่งกลับ แต่มิติที่สองมีความยาวเพียงอย่างเดียว 
เมื่อต้องการใช้ฟังก์ชันก่อนอื่นให้ตรวจดูว่าผลลัพธ์เป็นโมฆะหรือไม่ ถ้าผลลัพธ์เป็นโมฆะลำดับจะไม่ตรงกันเลย ถ้าลำดับไม่ตรงกันอาร์เรย์ 2D จะถูกส่งกลับ 
หากมีกลุ่ม (ระบุโดยวงเล็บ) ในนิพจน์ทั่วไปเนื้อหาของแต่ละรายการจะถูกส่งกลับในอาร์เรย์ สมมติว่าลูปมีตัวแปรตัวนับ i องค์ประกอบ [i] [0] ของการจับคู่นิพจน์ทั่วไปจะส่งกลับสตริงที่ตรงกันทั้งหมดและกลุ่มการจับคู่เริ่มต้นที่องค์ประกอบ [i] [1] (กลุ่มแรกคือ [i] [1] , ที่สอง [i] [2] และอื่น ๆ )

.. This function is used to apply a regular expression to a piece of text,
.. and return a list of matching groups (elements found inside parentheses)
.. as a two-dimensional String array. If there are no matches, a null value
.. will be returned. If no groups are specified in the regular expression,
.. but the sequence matches, a two dimensional array is still returned, but
.. the second dimension is only of length one.
.. 
.. To use the function, first check to see if the result is null. If the
.. result is null, then the sequence did not match at all. If the sequence
.. did match, a 2D array is returned.
.. 
.. If there are groups (specified by sets of parentheses) in the regular
.. expression, then the contents of each will be returned in the array.
.. Assuming a loop with counter variable i, element [i][0] of a regular
.. expression match returns the entire matching string, and the match groups
.. start at element [i][1] (the first group is [i][1], the second [i][2],
.. and so on).

**รูปแบบการใช้งาน**

matchAll ( str, regexp )

**พารามิเตอร์**

- ``str``  String: สตริงที่จะค้นหา

- ``regexp``  String: regexp ที่จะใช้สำหรับการจับคู่

.. ``str``  String: the String to be searched
.. ``regexp``  String: the regexp to be used for matching

**ค่าที่ส่งออกมา**

- Array.<String>: ค้นพบอาร์เรย์สตริง 2 สตริง

.. Array.<String>: 2d Array of Strings found

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var string = "Hello p5js*! Hello world!"
	var regexp = "Hello"
	matchAll(string, regexp);

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

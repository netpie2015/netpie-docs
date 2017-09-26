.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

removeTokens()
==============

 ลบอักขระที่ระบุ (หรือ &quot;โทเค็น&quot;)  หากไม่มีการระบุคอลัมน์ระบบจะประมวลผลค่าในคอลัมน์และแถวทั้งหมด คอลัมน์ที่ระบุอาจมีการอ้างอิงโดยใช้รหัสหรือชื่อ 

.. Removes any of the specified characters (or "tokens").
..  If no column is specified, then the values in all columns and
..  rows are processed. A specific column may be referenced by
..  either its ID or title.

**รูปแบบการใช้งาน**

removeTokens ( chars, [column] )

**พารามิเตอร์**

- ``chars``  String: ลบอักขระที่จะลบออก

- ``column``  String,Number: หมายเลขคอลัมน์ (หมายเลข) หรือชื่อ (สตริง)

.. ``chars``  String: String listing characters to be removed
.. ``column``  String,Number: Column ID (number) or name (string)

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

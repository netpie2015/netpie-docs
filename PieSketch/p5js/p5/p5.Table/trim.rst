.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

trim()
======

การตัดแต่งที่นำทางและต่อท้ายช่องว่างเช่นช่องว่างและแท็บจากค่าตารางสตริง หากไม่มีการระบุคอลัมน์ค่าในคอลัมน์และแถวทั้งหมดจะถูกตัดแต่ง คอลัมน์ที่ระบุอาจมีการอ้างอิงโดยใช้รหัสหรือชื่อ

.. Trims leading and trailing whitespace, such as spaces and tabs,
..  from String table values. If no column is specified, then the
..  values in all columns and rows are trimmed. A specific column
..  may be referenced by either its ID or title.

**รูปแบบการใช้งาน**

trim ( column )

**พารามิเตอร์**

- ``column``  String,Number: หมายเลขคอลัมน์ (หมายเลข) หรือชื่อ (สตริง)

.. ``column``  String,Number: Column ID (number) or name (string)

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.

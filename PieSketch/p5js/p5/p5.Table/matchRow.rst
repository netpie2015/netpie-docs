.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

matchRow()
==========

ค้นหาแถวแรกในตารางที่ตรงกับนิพจน์ทั่วไปที่มีให้และส่งกลับการอ้างอิงไปยังแถวนั้น แม้ว่าจะมีแถวหลายแถวที่เป็นไปได้การจับคู่จะมีการส่งคืนเฉพาะแถวที่ตรงกันเท่านั้น คอลัมน์เพื่อค้นหาอาจระบุโดย ID หรือชื่อ

.. Finds the first row in the Table that matches the regular
..  expression provided, and returns a reference to that row.
..  Even if multiple rows are possible matches, only the first
..  matching row is returned. The column to search may be
..  specified by either its ID or title.
**รูปแบบการใช้งาน**

matchRow ( regexp, column )

**พารามิเตอร์**

- ``regexp``  String: นิพจน์ทั่วไปเพื่อให้ตรงกับ

- ``column``  String,Number: หมายเลขคอลัมน์ (หมายเลข) หรือชื่อ (สตริง)

.. ``regexp``  String: The regular expression to match
.. ``column``  String,Number: The column ID (number) or
                                  title (string)

**ค่าที่ส่งออกมา**

- p5.TableRow: วัตถุ TableRow

.. p5.TableRow: TableRow object

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

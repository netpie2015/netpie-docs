.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

setString()
===========

เก็บค่าสตริงไว้ในแถวและคอลัมน์ที่กำหนดไว้ของตาราง แถวถูกระบุโดย ID ของมันในขณะที่คอลัมน์อาจถูกระบุโดย ID หรือชื่อของ

.. Stores a String value in the Table's specified row and column.
.. The row is specified by its ID, while the column may be specified
.. by either its ID or title.

**รูปแบบการใช้งาน**

setString ( row, column, value )

**พารามิเตอร์**

- ``row``  Number: ID แถว

- ``column``  String,Number: คอลัมน์ ID (จำนวน) หรือชื่อ (สตริง)

- ``value``  String: ค่าที่จะกำหนด

.. ``row``  Number: row ID
.. ``column``  String,Number: column ID (Number) or title (String)
.. ``value``  String: value to assign

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

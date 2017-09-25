.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

matchRow()
==========

Finds the first row in the Table that matches the regular
 expression provided, and returns a reference to that row.
 Even if multiple rows are possible matches, only the first
 matching row is returned. The column to search may be
 specified by either its ID or title.

**รูปแบบการใช้งาน**

matchRow ( regexp, column )

**พารามิเตอร์**

- ``regexp``  String: The regular expression to match

- ``column``  String,Number: The column ID (number) or title (string)


**ค่าที่ส่งออกมา**

- p5.TableRow: TableRow object


.. toctree::


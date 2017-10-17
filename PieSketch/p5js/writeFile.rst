.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

writeFile()
===========

สร้างหยดข้อมูลไฟล์เป็น URL เพื่อเตรียมการดาวน์โหลด ยอมรับอาร์เรย์ของข้อมูลชื่อไฟล์และส่วนขยาย (ตัวเลือก) นี่เป็นฟังก์ชันส่วนตัวเพราะไม่มีการฟอร์แมต แต่ถูกใช้โดย saveStrings, saveJSON, saveTable เป็นต้น

.. Generate a blob of file data as a url to prepare for download.
..  Accepts an array of data, a filename, and an extension (optional).
..  This is a private function because it does not do any formatting,
..  but it is used by saveStrings, saveJSON, saveTable etc.

**รูปแบบการใช้งาน**

writeFile ( dataToDownload, filename, extension )

**พารามิเตอร์**

- ``dataToDownload``  Array: 

- ``filename``  String: 

- ``extension``  : 

.. ``dataToDownload``  Array: 
.. ``filename``  String: 
.. ``extension``  : 

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.

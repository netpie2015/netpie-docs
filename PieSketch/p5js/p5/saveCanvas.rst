.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

saveCanvas()
============

บันทึกผืนผ้าใบปัจจุบันเป็นภาพ ใน Safari จะเป็นการเปิดภาพในหน้าต่างและผู้ใช้ต้องระบุชื่อไฟล์ของตนเองใน save-as เบราเซอร์อื่น ๆ จะบันทึกไฟล์ทันทีหรือแจ้งผู้ใช้ด้วยหน้าต่างโต้ตอบ

.. Save the current canvas as an image. In Safari, this will open the
..  image in the window and the user must provide their own
..  filename on save-as. Other browsers will either save the
..  file immediately, or prompt the user with a dialogue window.

**รูปแบบการใช้งาน**

saveCanvas ( selectedCanvas, [filename], [extension] )

**พารามิเตอร์**

- ``selectedCanvas``  p5.Element,HTMLCanvasElement: ตัวแปรที่แสดงถึงผืนผ้าใบ html5 (optional)

- ``filename``  String: 

- ``extension``  String: &#39;jpg&#39; หรือ &#39;png&#39;

.. ``selectedCanvas``  p5.Element,HTMLCanvasElement: a variable representing a specific html5 canvas (optional)
.. ``filename``  String: 
.. ``extension``  String: 'jpg' or 'png'

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.

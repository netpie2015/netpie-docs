.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

setModified()
=============

วิธีช่วยเหลือสำหรับโหมดเว็บ GL เพื่อระบุว่ารูปภาพมีการเปลี่ยนแปลงหรือไม่เปลี่ยนแปลงนับตั้งแต่อัปโหลดครั้งล่าสุด การอัปโหลดพื้น gl จะทำให้ค่านี้เป็น false หลังจากอัปโหลดพื้นผิว

.. helper method for web GL mode to indicate that an image has been
.. changed or unchanged since last upload. gl texture upload will
.. set this value to false after uploading the texture.
**รูปแบบการใช้งาน**

setModified ( val )

**พารามิเตอร์**

- ``val``  boolean: กำหนดว่ารูปภาพจะถูกแก้ไขหรือไม่

.. ``val``  boolean: sets whether or not the image has been
modified.

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

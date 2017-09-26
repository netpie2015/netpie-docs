.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

isModified()
============

วิธีช่วยเหลือสำหรับโหมดเว็บ GL เพื่อดูว่ารูปภาพได้รับการแก้ไขแล้วหรืออาจจำเป็นต้องอัปโหลดใหม่ไปยังหน่วยความจำเนื้อระหว่างเฟรม

.. helper method for web GL mode to figure out if the image
.. has been modified and might need to be re-uploaded to texture
.. memory between frames.
**รูปแบบการใช้งาน**

isModified ( )

**ค่าที่ส่งออกมา**

- boolean: แบบบูลที่ระบุว่ารูปภาพมีการอัปเดตหรือแก้ไขตั้งแต่การอัปโหลดภาพพื้นผิวครั้งล่าสุด

.. boolean: a boolean indicating whether or not the image has been updated or modified since last texture upload.

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

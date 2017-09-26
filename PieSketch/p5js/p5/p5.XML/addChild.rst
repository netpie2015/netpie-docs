.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

addChild()
==========

ผนวกลูกใหม่เข้ากับองค์ประกอบ สามารถระบุเด็กได้ด้วยสตริงซึ่งจะใช้เป็นชื่อแท็กใหม่หรือเป็นการอ้างอิงถึงอ็อบเจ็กต์ p5.XML ที่มีอยู่ การอ้างถึงเด็กที่เพิ่งสร้างใหม่จะถูกส่งกลับเป็น object p5.XML

.. Appends a new child to the element. The child can be specified with
.. either a String, which will be used as the new tag's name, or as a
.. reference to an existing p5.XML object.
.. A reference to the newly created child is returned as an p5.XML object.
**รูปแบบการใช้งาน**

addChild ( a )

**พารามิเตอร์**

- ``a``  p5.XML: p5.XML Object ซึ่งจะเป็นลูกที่จะเพิ่ม

.. ``a``  p5.XML: p5.XML Object which will be the child to be added

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

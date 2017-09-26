.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

getChildren()
=============

ส่งคืนเด็กทั้งหมดขององค์ประกอบเป็นอาร์เรย์ของออบเจ็กต์ p5.XML เมื่อมีการระบุพารามิเตอร์ชื่อแล้วจะมีการส่งคืนเด็กทั้งหมดที่ตรงกับชื่อนั้น

.. Returns all of the element's children as an array of p5.XML objects. When
.. the name parameter is specified, then it will return all children that match
.. that name.
**รูปแบบการใช้งาน**

getChildren ( [name] )

**พารามิเตอร์**

- ``name``  String: ชื่อองค์ประกอบ

.. ``name``  String: element name

**ค่าที่ส่งออกมา**

- Array.<p5.XML>: เด็กขององค์ประกอบ

.. Array.<p5.XML>: children of the element

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

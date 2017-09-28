.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

createElement()
===============

สร้างอิลิเมนต์ด้วยแท็กที่ระบุใน DOM พร้อมด้วยเนื้อหาที่กำหนด ผนวกเข้ากับโหนดคอนเทนเนอร์หากมีการระบุไว้มิฉะนั้นจะต่อท้ายกับเนื้อหา

.. Creates element with given tag in the DOM with given content.
.. Appends to the container node if one is specified, otherwise
.. appends to body.

**รูปแบบการใช้งาน**

createElement ( tag, [content] )

**พารามิเตอร์**

- ``tag``  String: แท็กสำหรับองค์ประกอบใหม่

- ``content``  String: เนื้อหา html ที่จะแทรกลงในองค์ประกอบ

.. ``tag``  String: tag for the new element
.. ``content``  String: html content to be inserted into the element

**ค่าที่ส่งออกมา**

- Object,p5.Element: ชี้ไปที่ p5.Element ถือสร้างโหนด

.. Object,p5.Element: pointer to p5.Element holding created node

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var h2 = createElement('h2','im an h2 p5.element!');

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.

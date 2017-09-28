.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

child()
=======

แนบองค์ประกอบดังกล่าวกับเด็กไว้กับผู้ปกครองที่ระบุ ยอมรับ ID สตริงโหนด DOM หรือ p5.Element หากไม่มีการระบุอาร์เรย์จะมีการส่งคืนอาร์เรย์ของโหนด DOM ของเด็ก

.. Attaches the element  as a child to the parent specified.
.. Accepts either a string ID, DOM node, or p5.Element.
.. If no argument is specified, an array of children DOM nodes is returned.

**รูปแบบการใช้งาน**

child ( [child] )

**พารามิเตอร์**

- ``child``  String,Object,p5.Element: ID, โหนด DOM หรือ p5.Element เพื่อเพิ่มองค์ประกอบปัจจุบัน

.. ``child``  String,Object,p5.Element: the ID, DOM node, or p5.Element to add to the current element

**ค่าที่ส่งออกมา**

- p5.Element: 

.. p5.Element: 

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var div0 = createDiv('this is the parent');
	var div1 = createDiv('this is the child');
	div0.child(div1); // use p5.Element
	var div0 = createDiv('this is the parent');
	var div1 = createDiv('this is the child');
	div1.id('apples');
	div0.child('apples'); // use id
	var div0 = createDiv('this is the parent');
	var elt = document.getElementById('myChildDiv');
	div0.child(elt); // use element from page

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.

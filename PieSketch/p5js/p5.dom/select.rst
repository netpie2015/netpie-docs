.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

select()
========

ค้นหาหน้าเว็บสำหรับองค์ประกอบที่มี ID ชั้นเรียนหรือชื่อแท็ก (ใช้คำนำหน้า '#' หรือ '.' เพื่อระบุ ID หรือคลาสตามลำดับและไม่มีสำหรับแท็ก) และส่งคืนค่าเป็น p5.Element ถ้าชื่อชั้นหรือชื่อแท็กมีมากกว่า 1 องค์ประกอบจะส่งคืนเฉพาะองค์ประกอบแรกเท่านั้น โหนด DOM สามารถเข้าถึงได้โดยใช้ .elt ส่งกลับค่า null ถ้าไม่มีพบ นอกจากนี้คุณยังสามารถระบุคอนเทนเนอร์เพื่อค้นหาภายใน

.. Searches the page for an element with the given ID, class, or tag name (using the '#' or '.'
.. prefixes to specify an ID or class respectively, and none for a tag) and returns it as
.. a p5.Element. If a class or tag name is given with more than 1 element,
.. only the first element will be returned.
.. The DOM node itself can be accessed with .elt.
.. Returns null if none found. You can also specify a container to search within.

**รูปแบบการใช้งาน**

select ( name, [container] )

**พารามิเตอร์**

- ``name``  String: id, class หรือชื่อแท็กของ element ที่ต้องการค้นหา

- ``container``  String: id, p5.Element หรือ HTML เพื่อค้นหาภายใน

.. ``name``  String: id, class, or tag name of element to search for
.. ``container``  String: id, p5.Element, or HTML element to search within

**ค่าที่ส่งออกมา**

- Object,p5.Element,Null: p5.Element containing node พบแล้ว

.. Object,p5.Element,Null: p5.Element containing node found

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	<code class='norender'>
	function setup() {
	  createCanvas(100,100);
	  //translates canvas 50px down
	  select('canvas').position(100, 100);
	}
	<code class='norender'>
	// these are all valid calls to select()
	var a = select('#moo');
	var b = select('#blah', '#myContainer');
	var c = select('#foo', b);
	var d = document.getElementById('beep');
	var e = select('p', d);

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.

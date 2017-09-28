.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

selectAll()
===========

ค้นหาหน้าเว็บสำหรับองค์ประกอบที่มีชั้นหรือชื่อแท็ก (ใช้คำนำหน้า '.' เพื่อระบุคลาสและไม่มีคำนำหน้าสำหรับแท็ก) และส่งกลับค่าเป็น p5.Elements ในอาร์เรย์ โหนด DOM สามารถเข้าถึงได้โดยใช้ .elt ส่งกลับอาร์เรย์ที่ว่างเปล่าหากไม่มีพบ นอกจากนี้คุณยังสามารถระบุคอนเทนเนอร์เพื่อค้นหาภายใน

.. Searches the page for elements with the given class or tag name (using the '.' prefix
.. to specify a class and no prefix for a tag) and returns them as p5.Elements
.. in an array.
.. The DOM node itself can be accessed with .elt.
.. Returns an empty array if none found.
.. You can also specify a container to search within.

**รูปแบบการใช้งาน**

selectAll ( name, [container] )

**พารามิเตอร์**

- ``name``  String: คลาสหรือชื่อแท็กขององค์ประกอบที่จะค้นหา

- ``container``  String: id, p5.Element หรือ HTML เพื่อค้นหาภายใน

.. ``name``  String: class or tag name of elements to search for
.. ``container``  String: id, p5.Element, or HTML element to search within

**ค่าที่ส่งออกมา**

- Array: อาร์เรย์ของ p5.Elements ที่มีโหนดพบ

.. Array: Array of p5.Elements containing nodes found

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	  createButton('btn');
	  createButton('2nd btn');
	  createButton('3rd btn');
	  var buttons = selectAll('button');
	
	  for (var i = 0; i < buttons.length; i++){
	    buttons[i].size(100,100);
	  }
	}
	// these are all valid calls to selectAll()
	var a = selectAll('.moo');
	var b = selectAll('div');
	var c = selectAll('button', '#myContainer');
	var d = select('#container');
	var e = selectAll('p', d);
	var f = document.getElementById('beep');
	var g = select('.blah', f);

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.

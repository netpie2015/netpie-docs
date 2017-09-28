.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

createSelect()
==============

สร้างเมนูแบบเลื่อนลง   ใน DOM นอกจากนี้ยังช่วยในการกำหนดวิธีการเลือกกล่องเพื่อ p5.Element เมื่อเลือกกล่องเลือกที่มีอยู่

.. Creates a dropdown menu &lt;select&gt;&lt;/select&gt; element in the DOM.
.. It also helps to assign select-box methods to p5.Element when selecting existing select box

**รูปแบบการใช้งาน**

createSelect ( [multiple] )

**พารามิเตอร์**

- ``multiple``  boolean: จริงถ้าเมนูแบบเลื่อนลงควรสนับสนุนการเลือกหลายรายการ

.. ``multiple``  boolean: true if dropdown should support multiple selections

**ค่าที่ส่งออกมา**

- p5.Element: 

.. p5.Element: 

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var sel;
	
	function setup() {
	  textAlign(CENTER);
	  background(200);
	  sel = createSelect();
	  sel.position(10, 10);
	  sel.option('pear');
	  sel.option('kiwi');
	  sel.option('grape');
	  sel.changed(mySelectEvent);
	}
	
	function mySelectEvent() {
	  var item = sel.value();
	  background(200);
	  text("it's a "+item+"!", 50, 50);
	}

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.

.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

createP()
=========

สร้างอิลิเมนต์   ใน DOM พร้อมด้วย HTML ภายใน ใช้สำหรับข้อความความยาววรรค ผนวกเข้ากับโหนดคอนเทนเนอร์หากมีการระบุไว้มิฉะนั้นจะต่อท้ายกับเนื้อหา

.. Creates a &lt;p&gt;&lt;/p&gt; element in the DOM with given inner HTML. Used
.. for paragraph length text.
.. Appends to the container node if one is specified, otherwise
.. appends to body.

**รูปแบบการใช้งาน**

createP ( [html] )

**พารามิเตอร์**

- ``html``  String: HTML ภายในสำหรับองค์ประกอบที่สร้างขึ้น

.. ``html``  String: inner HTML for element created

**ค่าที่ส่งออกมา**

- Object,p5.Element: ชี้ไปที่ p5.Element ถือสร้างโหนด

.. Object,p5.Element: pointer to p5.Element holding created node

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var myP;
	function setup() {
	  myP = createP('this is some text');
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

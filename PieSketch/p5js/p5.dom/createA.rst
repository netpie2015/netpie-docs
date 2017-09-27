.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

createA()
=========

สร้าง   องค์ประกอบใน DOM สำหรับใส่ไฮเปอร์ลิงก์ ผนวกเข้ากับโหนดคอนเทนเนอร์หากมีการระบุไว้มิฉะนั้นจะต่อท้ายกับเนื้อหา

.. Creates an &lt;a&gt;&lt;/a&gt; element in the DOM for including a hyperlink.
.. Appends to the container node if one is specified, otherwise
.. appends to body.

**รูปแบบการใช้งาน**

createA ( href, html, [target] )

**พารามิเตอร์**

- ``href``  String: url ของหน้าเว็บที่จะเชื่อมโยงไป

- ``html``  String: html ภายในขององค์ประกอบลิงก์ที่จะแสดง

- ``target``  String: เป้าหมายที่จะเปิดลิงก์ใหม่อาจเป็น _blank, _self, _parent, _top

.. ``href``  String: url of page to link to
.. ``html``  String: inner html of link element to display
.. ``target``  String: target where new link should open, could be _blank, _self, _parent, _top.

**ค่าที่ส่งออกมา**

- Object,p5.Element: ชี้ไปที่ p5.Element ถือสร้างโหนด

.. Object,p5.Element: pointer to p5.Element holding created node

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var myLink;
	function setup() {
	  myLink = createA('http://p5js.org/', 'this is a link');
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

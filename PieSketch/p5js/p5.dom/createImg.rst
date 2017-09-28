.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

createImg()
===========

สร้างอิลิเมนต์  ใน DOM พร้อมด้วย src และข้อความสำรอง ผนวกเข้ากับโหนดคอนเทนเนอร์หากมีการระบุไว้มิฉะนั้นจะต่อท้ายกับเนื้อหา

.. Creates an &lt;img&gt; element in the DOM with given src and
.. alternate text.
.. Appends to the container node if one is specified, otherwise
.. appends to body.

**รูปแบบการใช้งาน**

createImg ( src, [alt], [successCallback] )

**พารามิเตอร์**

- ``src``  String: src เส้นทางหรือ URL สำหรับภาพ

- ``alt``  String: ข้อความอื่นที่จะใช้หากไม่ได้โหลดรูปภาพ

- ``successCallback``  function: เรียกกลับเมื่อมีการเรียกข้อมูลภาพ

.. ``src``  String: src path or url for image
.. ``alt``  String: alternate text to be used if image does not load
.. ``successCallback``  function: callback to be called once image data is loaded

**ค่าที่ส่งออกมา**

- Object,p5.Element: ชี้ไปที่ p5.Element ถือสร้างโหนด

.. Object,p5.Element: pointer to p5.Element holding created node

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var img;
	function setup() {
	  img = createImg('http://p5js.org/img/asterisk-01.png');
	}

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.

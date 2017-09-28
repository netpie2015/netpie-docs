.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

createInput()
=============

สร้างอิลิเมนต์   ใน DOM สำหรับป้อนข้อความ ใช้ขนาด. () เพื่อกำหนดความยาวของช่อง ผนวกเข้ากับโหนดคอนเทนเนอร์หากมีการระบุไว้มิฉะนั้นจะต่อท้ายกับเนื้อหา

.. Creates an &lt;input&gt;&lt;/input&gt; element in the DOM for text input.
.. Use .size() to set the display length of the box.
.. Appends to the container node if one is specified, otherwise
.. appends to body.

**รูปแบบการใช้งาน**

createInput ( [value], [type] )

**พารามิเตอร์**

- ``value``  Number: ค่าดีฟอลต์ของช่องใส่

- ``type``  String: ประเภทของข้อความเช่นข้อความรหัสผ่าน ฯลฯ ค่าเริ่มต้นเป็นข้อความ

.. ``value``  Number: default value of the input box
.. ``type``  String: type of text, ie text, password etc. Defaults to text

**ค่าที่ส่งออกมา**

- Object,p5.Element: ชี้ไปที่ p5.Element ถือสร้างโหนด

.. Object,p5.Element: pointer to p5.Element holding created node

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup(){
	  var inp = createInput('');
	  inp.input(myInputEvent);
	}
	
	function myInputEvent(){
	  console.log('you are typing: ', this.value());
	}
	

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.

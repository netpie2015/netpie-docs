.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

createFileInput()
=================

สร้างอิลิเมนต์   ใน DOM ของชนิด 'file' ซึ่งจะช่วยให้ผู้ใช้สามารถเลือกไฟล์ในเครื่องสำหรับใช้ในการร่าง

.. Creates an &lt;input&gt;&lt;/input&gt; element in the DOM of type 'file'.
.. This allows users to select local files for use in a sketch.

**รูปแบบการใช้งาน**

createFileInput ( [callback], [multiple] )

**พารามิเตอร์**

- ``callback``  function: ฟังก์ชันเรียกกลับเมื่อโหลดไฟล์

- ``multiple``  String: เลือกเพื่ออนุญาตให้มีไฟล์หลายไฟล์

.. ``callback``  function: callback function for when a file loaded
.. ``multiple``  String: optional to allow multiple files selected

**ค่าที่ส่งออกมา**

- Object,p5.Element: ชี้ไปที่ p5.Element ถือสร้างองค์ประกอบ DOM

.. Object,p5.Element: pointer to p5.Element holding created DOM element

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var input;
	var img;
	
	function setup() {
	  input = createFileInput(handleFile);
	  input.position(0, 0);
	}
	
	function draw() {
	  if (img) {
	    image(img, 0, 0, width, height);
	  }
	}
	
	function handleFile(file) {
	  print(file);
	  if (file.type === 'image') {
	    img = createImg(file.data);
	    img.hide();
	  }
	}

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.

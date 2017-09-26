.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

loadFont()
==========

โหลดไฟล์ font opentype (.otf, .ttf) จากไฟล์หรือ URL และส่งคืนออบเจ็กต์ PFont วิธีนี้ไม่ตรงกันซึ่งหมายความว่าอาจไม่เสร็จสิ้นก่อนที่จะดำเนินการบรรทัดถัดไปในร่างของคุณ 
เส้นทางไปยังแบบอักษรควรเทียบกับไฟล์ HTML ที่ลิงก์ในร่างของคุณ การโหลด URL จากที่อยู่ระยะไกลหรืออื่น ๆ อาจถูกบล็อกเนื่องจากความปลอดภัยในตัวของเบราเซอร์

.. Loads an opentype font file (.otf, .ttf) from a file or a URL,
.. and returns a PFont Object. This method is asynchronous,
.. meaning it may not finish before the next line in your sketch
.. is executed.
.. 
.. The path to the font should be relative to the HTML file
.. that links in your sketch. Loading an from a URL or other
.. remote location may be blocked due to your browser's built-in
.. security.
**รูปแบบการใช้งาน**

loadFont ( path, [callback] )

**พารามิเตอร์**

- ``path``  String: ชื่อไฟล์หรือ URL ที่จะโหลด

- ``callback``  function: ฟังก์ชันที่จะดำเนินการหลังจาก loadFont () เสร็จสิ้น

.. ``path``  String: name of the file or url to load
.. ``callback``  function: function to be executed after
                                   loadFont()
                                   completes

**ค่าที่ส่งออกมา**

- p5.Font: p5.Font object

.. p5.Font: p5.Font object

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	<p>Calling loadFont() inside preload() guarantees that the load
	operation will have completed before setup() and draw() are called.</p>
	
	var myFont;
	function preload() {
	  myFont = loadFont('assets/AvenirNextLTPro-Demi.otf');
	}
	
	function setup() {
	  fill('#ED225D');
	  textFont(myFont);
	  textSize(36);
	  text('p5*js', 10, 50);
	}
	Outside of preload(), you may supply a callback function to handle the
	object:
	
	function setup() {
	  loadFont('assets/AvenirNextLTPro-Demi.otf', drawText);
	}
	
	function drawText(font) {
	  fill('#ED225D');
	  textFont(font, 36);
	  text('p5*js', 10, 50);
	}
	
	<p>You can also use the string name of the font to style other HTML
	elements.</p>
	
	var myFont;
	
	function preload() {
	  myFont = loadFont('assets/Avenir.otf');
	}
	
	function setup() {
	  var myDiv = createDiv('hello there');
	  myDiv.style('font-family', 'Avenir');
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

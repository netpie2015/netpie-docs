.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

drop()
======

มีการเรียกใช้ฟังก์ชัน. drop () สำหรับแต่ละไฟล์ที่ลดลงในองค์ประกอบ ต้องมีการเรียกกลับที่ส่งผ่านวัตถุ p5.File คุณสามารถส่งผ่าน callbacks ได้สองรายการโดยจะเรียกใช้งานครั้งแรก (ต้องระบุ) สำหรับแต่ละไฟล์ที่ลดลงเมื่อโหลดไฟล์ วินาที (ตัวเลือก) จะถูกเรียกใช้งานเพียงครั้งเดียวเมื่อไฟล์ (หรือไฟล์) ถูกทิ้ง

.. The .drop() function is called for each file dropped on the element.
.. It requires a callback that is passed a p5.File object.  You can
.. optionally pass two callbacks, the first one (required) is triggered
.. for each file dropped when the file is loaded.  The second (optional)
.. is triggered just once when a file (or files) are dropped.

**รูปแบบการใช้งาน**

drop ( callback, fxn )

**พารามิเตอร์**

- ``callback``  function: เรียกกลับเมื่อไฟล์ถูกทิ้ง

- ``fxn``  function: เรียกกลับเพื่อรับไฟล์ที่โหลด

.. ``callback``  function: callback triggered when files are dropped.
.. ``fxn``  function: callback to receive loaded file.

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	  var c = createCanvas(100, 100);
	  background(200);
	  textAlign(CENTER);
	  text('drop image', width/2, height/2);
	  c.drop(gotFile);
	}
	
	function gotFile(file) {
	  var img = createImg(file.data).hide();
	  // Draw the image onto the canvas
	  image(img, 0, 0, width, height);
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

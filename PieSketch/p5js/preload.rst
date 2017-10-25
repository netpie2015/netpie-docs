.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

preload()
=========

เรียกก่อนโดยตรง () ฟังก์ชัน preload () ใช้เพื่อจัดการการโหลดข้อมูลภายนอกแบบอะซิงโครนัส หากมีการกำหนดฟังก์ชั่น preload ขึ้นมา setup () จะรอจนกว่าจะมีการเรียกใช้งานโหลดเสร็จสิ้น ไม่มีอะไรนอกจากการโหลดควรอยู่ภายในโหลดก่อน (loadImage, loadJSON, loadFont, loadStrings ฯลฯ )

โดยค่าเริ่มต้นข้อความ "loading ... " จะปรากฏขึ้น หากต้องการสร้างหน้าการโหลดของคุณเองให้ใส่องค์ประกอบ HTML ที่มีรหัส "p5_loading" ในหน้าเว็บของคุณ

.. Called directly before setup(), the preload() function is used to handle asynchronous loading of external files. If a preload function is defined, setup() will wait until any load calls within have finished. Nothing besides load calls should be inside preload (loadImage, loadJSON, loadFont, loadStrings, etc).
.. By default the text "loading..." will be displayed. To make your own loading page, include an HTML element with id "p5_loading" in your page.

**รูปแบบการใช้งาน**

preload()

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var img;
    var c;
    function preload() {  // preload() runs once
    img = loadImage('assets/laDefense.jpg');
    }

    function setup() {  // setup() waits until preload() is done
    img.loadPixels();
    // get color of middle pixel
    c = img.get(img.width/2, img.height/2);
    }

    function draw() {
    background(c);
    image(img, 25, 25, 50, 50);
    }
	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.

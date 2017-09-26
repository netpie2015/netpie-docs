.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

loadPixels()
============

โหลดข้อมูลพิกเซลสำหรับภาพนี้ลงในแอตทริบิวต์ [pixels]

.. Loads the pixels data for this image into the [pixels] attribute.

**รูปแบบการใช้งาน**

loadPixels ( )

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var myImage;
	var halfImage;
	
	function preload() {
	  myImage = loadImage("assets/rockies.jpg");
	}
	
	function setup() {
	  myImage.loadPixels();
	  halfImage = 4 * width * height/2;
	  for(var i = 0; i < halfImage; i++){
	    myImage.pixels[i+halfImage] = myImage.pixels[i];
	  }
	  myImage.updatePixels();
	}
	
	function draw() {
	  image(myImage, 0, 0);
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

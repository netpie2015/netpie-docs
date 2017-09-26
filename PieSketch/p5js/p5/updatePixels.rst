.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

updatePixels()
==============

อัพเดตหน้าต่างแสดงผลด้วยข้อมูลในอาร์เรย์พิกเซล [] ใช้ร่วมกับ loadPixels () หากคุณกำลังอ่านพิกเซลจากอาร์เรย์เพียงอย่างเดียวไม่จำเป็นต้องเรียกใช้ updatePixels () - การอัปเดตเป็นสิ่งจำเป็นเท่านั้นเพื่อใช้การเปลี่ยนแปลง updatePixels () ควรถูกเรียกเมื่อใดก็ตามที่มีการจัดการหรือตั้งค่าอาร์เรย์พิกเซล () และจะมีการเปลี่ยนแปลงเฉพาะกับ set () หรือการเปลี่ยนแปลงโดยตรงไปยังพิกเซล [] เท่านั้น

.. Updates the display window with the data in the pixels[] array.
.. Use in conjunction with loadPixels(). If you're only reading pixels from
.. the array, there's no need to call updatePixels() — updating is only
.. necessary to apply changes. updatePixels() should be called anytime the
.. pixels array is manipulated or set() is called, and only changes made with
.. set() or direct changes to pixels[] will occur.

**รูปแบบการใช้งาน**

updatePixels ( [x], [y], [w], [h] )

**พารามิเตอร์**

- ``x``  Number: x พิกัดของมุมซ้ายบนของพื้นที่เพื่อปรับปรุง

- ``y``  Number: y พิกัดของมุมบนซ้ายของพื้นที่เพื่อปรับปรุง

- ``w``  Number: ความกว้างของพื้นที่ที่จะปรับปรุง

- ``h``  Number: ความสูงของพื้นที่ที่จะอัปเดต

.. ``x``  Number: x-coordinate of the upper-left corner of region to update
.. ``y``  Number: y-coordinate of the upper-left corner of region to update
.. ``w``  Number: width of region to update
.. ``h``  Number: height of region to update

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var img;
	function preload() {
	  img = loadImage("assets/rockies.jpg");
	}
	
	function setup() {
	  image(img, 0, 0);
	  var halfImage = 4 * (img.width * pixelDensity()) *
	    (img.height * pixelDensity()/2);
	  loadPixels();
	  for (var i = 0; i < halfImage; i++) {
	    pixels[i+halfImage] = pixels[i];
	  }
	  updatePixels();
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

set()
=====

 เปลี่ยนสีของพิกเซลใด ๆ หรือเขียนภาพโดยตรงไปยังหน้าต่างแสดงผล  พารามิเตอร์ x และ y ระบุพิกเซลที่จะเปลี่ยนแปลงและพารามิเตอร์ c ระบุค่าสี ซึ่งอาจเป็นวัตถุ p5.Color หรืออาร์เรย์พิกเซล [R, G, B, A] นอกจากนี้ยังสามารถเป็นค่าสีเทาเดียว เมื่อตั้งค่ารูปภาพพารามิเตอร์ x และ y จะกำหนดพิกัดสำหรับมุมซ้ายบนของภาพโดยไม่คำนึงถึง imageMode () ปัจจุบัน  หลังจากใช้ set () คุณต้องเรียกใช้ updatePixels () เพื่อให้การเปลี่ยนแปลงของคุณปรากฏขึ้น ควรจะเรียกว่าเมื่อมีการตั้งค่าพิกเซลทั้งหมดและต้องเรียกก่อนโทรหา () หรือวาดรูป  การตั้งค่าสีของพิกเซลเดียวด้วยชุด (x, y) เป็นเรื่องง่าย แต่ไม่เร็วเท่าการวางข้อมูลลงในพิกเซล [] การตั้งค่าพิกเซล [] โดยตรงอาจซับซ้อนเมื่อทำงานกับจอแสดงผลเรตินา แต่จะทำงานได้ดีขึ้นเมื่อต้องตั้งค่าพิกเซลจำนวนมากให้ตรงกับทุกลูป  ดูข้อมูลอ้างอิงสำหรับพิกเซล [] สำหรับข้อมูลเพิ่มเติม 

.. Changes the color of any pixel, or writes an image directly to the
.. display window.
.. The x and y parameters specify the pixel to change and the c parameter
.. specifies the color value. This can be a p5.Color object, or [R, G, B, A]
.. pixel array. It can also be a single grayscale value.
.. When setting an image, the x and y parameters define the coordinates for
.. the upper-left corner of the image, regardless of the current imageMode().
.. 
.. 
.. After using set(), you must call updatePixels() for your changes to appear.
.. This should be called once all pixels have been set, and must be called before
.. calling .get() or drawing the image.
.. 
.. Setting the color of a single pixel with set(x, y) is easy, but not as
.. fast as putting the data directly into pixels[]. Setting the pixels[]
.. values directly may be complicated when working with a retina display,
.. but will perform better when lots of pixels need to be set directly on
.. every loop.
.. See the reference for pixels[] for more information.

**รูปแบบการใช้งาน**

set ( x, y, c )

**พารามิเตอร์**

- ``x``  Number: พิกัด x ของพิกเซล

- ``y``  Number: y พิกัดของพิกเซล

- ``c``  Number,Array,Object: ใส่ค่า grayscale | อาร์เรย์พิกเซล | วัตถุ p5.Color | p5.Image to copy

.. ``x``  Number: x-coordinate of the pixel
.. ``y``  Number: y-coordinate of the pixel
.. ``c``  Number,Array,Object: insert a grayscale value | a pixel array | a p5.Color object | a p5.Image to copy

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var black = color(0);
	set(30, 20, black);
	set(85, 20, black);
	set(85, 75, black);
	set(30, 75, black);
	updatePixels();

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	for (var i = 30; i < width-15; i++) {
	  for (var j = 20; j < height-25; j++) {
	    var c = color(204-j, 153-i, 0);
	    set(i, j, c);
	  }
	}
	updatePixels();

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	var img;
	function preload() {
	  img = loadImage("assets/rockies.jpg");
	}
	
	function setup() {
	  set(0, 0, img);
	  updatePixels();
	  line(0, 0, width, height);
	  line(0, height, width, 0);
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

pixels
========

อาร์เรย์ที่มีค่าสำหรับพิกเซลทั้งหมดในหน้าต่างที่แสดง ค่าเหล่านี้คือตัวเลข อาร์เรย์นี้เป็นขนาด (รวมถึงปัจจัยที่เหมาะสมสำหรับ pixelDensity) ของหน้าต่างแสดง x4 แทนค่า R, G, B, A เพื่อให้แต่ละพิกเซลเคลื่อนที่จากซ้ายไปขวาในแต่ละแถวจากนั้นให้ลดแต่ละคอลัมน์ เรตินาและจอแสดงผลที่มีความละเอียดสูงอื่น ๆ อาจมีพิกเซลมากขึ้น [] (โดยค่าพิกเซลความหนาแน่น = 2) ตัวอย่างเช่นถ้าภาพมีขนาด 100x100 พิกเซลจะมี 40,000 ภาพ ด้วย pixelDensity = 2 จะมี 160,000 สี่ค่าแรก (ดัชนี 0-3) ในอาร์เรย์จะเป็นค่า R, G, B, A ของพิกเซลที่ (0, 0) ค่าที่สองสี่ (ดัชนี 4-7) จะมีค่า R, G, B, A ของพิกเซลที่ (1, 0) โดยทั่วไปในการตั้งค่าพิกเซลที่ (x, y): `` javascript var d = pixelDensity; สำหรับ (var i = 0; i <d; i ++) {สำหรับ (var j = 0; j <d; j ++) {// วนรอบ idx = 4 * ((y * d + j) * width * d + ( x * d + i)); พิกเซล [idx] = r; พิกเซล [idx + 1] = g; พิกเซล [idx + 2] = b; พิกเซล [idx + 3] = a; }} `` ` 
ก่อนที่จะเข้าถึงอาร์เรย์นี้ข้อมูลต้องโหลดด้วยฟังก์ชัน loadPixels () หลังจากที่ข้อมูลอาร์เรย์ได้รับการแก้ไขต้องใช้ฟังก์ชัน updatePixels () เพื่ออัพเดตการเปลี่ยนแปลง

.. Array containing the values for all the pixels in the display window.
.. These values are numbers. This array is the size (include an appropriate
.. factor for pixelDensity) of the display window x4,
.. representing the R, G, B, A values in order for each pixel, moving from
.. left to right across each row, then down each column. Retina and other
.. high denisty displays may have more pixels[] (by a factor of
.. pixelDensity^2).
.. For example, if the image is 100x100 pixels, there will be 40,000. With
.. pixelDensity = 2, there will be 160,000. The first four values
.. (indices 0-3) in the array will be the R, G, B, A values of the pixel at
.. (0, 0). The second four values (indices 4-7) will contain the R, G, B, A
.. values of the pixel at (1, 0). More generally, to set values for a pixel
.. at (x, y):
.. ```javascript
.. var d = pixelDensity;
.. for (var i = 0; i < d; i++) {
..   for (var j = 0; j < d; j++) {
..     // loop over
..     idx = 4 * ((y * d + j) * width * d + (x * d + i));
..     pixels[idx] = r;
..     pixels[idx+1] = g;
..     pixels[idx+2] = b;
..     pixels[idx+3] = a;
..   }
.. }
.. ```
.. 
.. Before accessing this array, the data must loaded with the loadPixels()
.. function. After the array data has been modified, the updatePixels()
.. function must be run to update the changes.

**รูปแบบการใช้งาน**

pixels

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	img = createImage(66, 66);
	img.loadPixels();
	for (i = 0; i < img.width; i++) {
	  for (j = 0; j < img.height; j++) {
	    img.set(i, j, color(0, 90, 102));
	  }
	}
	img.updatePixels();
	image(img, 17, 17);

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var pink = color(255, 102, 204);
	img = createImage(66, 66);
	img.loadPixels();
	for (var i = 0; i < 4*(width*height/2); i+=4) {
	  img.pixels[i] = red(pink);
	  img.pixels[i+1] = green(pink);
	  img.pixels[i+2] = blue(pink);
	  img.pixels[i+3] = alpha(pink);
	}
	img.updatePixels();
	image(img, 17, 17);

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.

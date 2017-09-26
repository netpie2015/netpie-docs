.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

pixels
========

Uint8ClampedArray มีค่าสำหรับพิกเซลทั้งหมดในหน้าต่างแสดงผล ค่าเหล่านี้คือตัวเลข อาร์เรย์นี้เป็นขนาด (รวมถึงปัจจัยที่เหมาะสมสำหรับ pixelDensity) ของหน้าต่างแสดง x4 แทนค่า R, G, B, A เพื่อให้แต่ละพิกเซลเคลื่อนที่จากซ้ายไปขวาในแต่ละแถวจากนั้นให้ลดแต่ละคอลัมน์ Retina และการแสดงความหนาแน่นสูงอื่น ๆ จะมีพิกเซลมากขึ้น [] (โดย pixelDensity ^ 2) ตัวอย่างเช่นถ้าภาพมีขนาด 100x100 พิกเซลจะมี 40,000 ภาพ บนจอแสดงผลจอตาจะมี 160,000 ราย 
สี่ค่าแรก (ดัชนี 0-3) ในอาร์เรย์จะเป็นค่า R, G, B, A ของพิกเซลที่ (0, 0) ค่าที่สองสี่ (ดัชนี 4-7) จะมีค่า R, G, B, A ของพิกเซลที่ (1, 0) โดยทั่วไปในการกำหนดค่าสำหรับพิกเซลที่ (x, y): `` javascript var d = pixelDensity (); สำหรับ (var i = 0; i &lt;d; i ++) {สำหรับ (var j = 0; j &lt;d; j ++) {// วนรอบ idx = 4 * ((y * d + j) * width * d + ( x * d + i)); พิกเซล [idx] = r; พิกเซล [idx + 1] = g; พิกเซล [idx + 2] = b; พิกเซล [idx + 3] = a; }} `` `  แม้ว่าวิธีการข้างต้นจะมีความซับซ้อน แต่ก็มีความยืดหยุ่นพอที่จะทำงานร่วมกับ pixelDensity ใดก็ได้ โปรดทราบว่า set () จะดูแลการตั้งค่าที่เหมาะสมทั้งหมดเป็นพิกเซล [] สำหรับค่าที่กำหนด (x, y) ที่ pixelDensity ใด ๆ แต่ประสิทธิภาพอาจไม่เร็วเท่าที่เมื่อมีการปรับเปลี่ยนค่าพิกเซลมาก 
ก่อนที่จะเข้าถึงอาร์เรย์นี้ข้อมูลต้องโหลดด้วยฟังก์ชัน loadPixels () หลังจากที่ข้อมูลอาร์เรย์ได้รับการแก้ไขต้องใช้ฟังก์ชัน updatePixels () เพื่ออัพเดตการเปลี่ยนแปลง 
โปรดทราบว่านี่ไม่ใช่อาร์เรย์ javascript มาตรฐาน ซึ่งหมายความว่าฟังก์ชันจาวาสคริปต์มาตรฐานเช่น slice() หรือ arrayCopy() ไม่ทำงาน 

.. Uint8ClampedArray
.. containing the values for all the pixels in the display window.
.. These values are numbers. This array is the size (include an appropriate
.. factor for pixelDensity) of the display window x4,
.. representing the R, G, B, A values in order for each pixel, moving from
.. left to right across each row, then down each column. Retina and other
.. high density displays will have more pixels[] (by a factor of
.. pixelDensity^2).
.. For example, if the image is 100x100 pixels, there will be 40,000. On a
.. retina display, there will be 160,000.
.. 
.. The first four values (indices 0-3) in the array will be the R, G, B, A
.. values of the pixel at (0, 0). The second four values (indices 4-7) will
.. contain the R, G, B, A values of the pixel at (1, 0). More generally, to
.. set values for a pixel at (x, y):
.. ```javascript
.. var d = pixelDensity();
.. for (var i = 0; i While the above method is complex, it is flexible enough to work with
.. any pixelDensity. Note that set() will automatically take care of
.. setting all the appropriate values in pixels[] for a given (x, y) at
.. any pixelDensity, but the performance may not be as fast when lots of
.. modifications are made to the pixel array.
.. 
.. Before accessing this array, the data must loaded with the loadPixels()
.. function. After the array data has been modified, the updatePixels()
.. function must be run to update the changes.
.. 
.. Note that this is not a standard javascript array.  This means that
.. standard javascript functions such as slice() or
.. arrayCopy() do not
.. work.

**รูปแบบการใช้งาน**

pixels

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var pink = color(255, 102, 204);
	loadPixels();
	var d = pixelDensity();
	var halfImage = 4 * (width * d) * (height/2 * d);
	for (var i = 0; i < halfImage; i+=4) {
	  pixels[i] = red(pink);
	  pixels[i+1] = green(pink);
	  pixels[i+2] = blue(pink);
	  pixels[i+3] = alpha(pink);
	}
	updatePixels();

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

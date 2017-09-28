.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

noiseDetail()
=============

ปรับตัวอักษรและระดับของรายละเอียดที่ผลิตโดยฟังก์ชัน Perlin noise คล้ายคลึงกับฮาร์โมนิกในฟิสิกส์เสียงจะถูกคำนวณในหลายอ็อกเตฟ อ็อกเทลด้านล่างมีส่วนร่วมกับสัญญาณเอาท์พุทมากขึ้นและเป็นตัวกำหนดความเข้มโดยรวมของเสียงขณะที่โอเว่อร์ที่สูงขึ้นจะสร้างรายละเอียดปลีกย่อยในลำดับสัญญาณรบกวน 
โดยค่าเริ่มต้นเสียงจะถูกคำนวณมากกว่า 4 โอห์เลสก์ซึ่งแต่ละคู่มีสัดส่วนครึ่งหนึ่งมากกว่ารุ่นก่อนเริ่มต้นที่ความแรง 50% สำหรับช่วง 1 วินาที จำนวน falloff นี้สามารถเปลี่ยนแปลงได้โดยการเพิ่มพารามิเตอร์ฟังก์ชันเพิ่มเติม เช่น. ปัจจัย falloff เท่ากับ 0.75 หมายความว่าแต่ละ octave จะมีผลกระทบ 75% (25% น้อยกว่า) ของระดับต่ำสุดก่อนหน้านี้ ค่าใด ๆ ระหว่าง 0.0 ถึง 1.0 เป็นค่าที่ถูกต้อง แต่โปรดทราบว่าค่าที่มากกว่า 0.5 อาจทำให้มีค่ามากกว่า 1.0 จาก เสียง () 
โดยการเปลี่ยนพารามิเตอร์เหล่านี้สัญญาณที่สร้างโดยฟังก์ชัน noise () สามารถปรับให้เหมาะกับความต้องการและลักษณะเฉพาะที่เฉพาะเจาะจงมาก

.. Adjusts the character and level of detail produced by the Perlin noise
.. function. Similar to harmonics in physics, noise is computed over
.. several octaves. Lower octaves contribute more to the output signal and
.. as such define the overall intensity of the noise, whereas higher octaves
.. create finer grained details in the noise sequence.
.. 
.. By default, noise is computed over 4 octaves with each octave contributing
.. exactly half than its predecessor, starting at 50% strength for the 1st
.. octave. This falloff amount can be changed by adding an additional function
.. parameter. Eg. a falloff factor of 0.75 means each octave will now have
.. 75% impact (25% less) of the previous lower octave. Any value between
.. 0.0 and 1.0 is valid, however note that values greater than 0.5 might
.. result in greater than 1.0 values returned by noise().
.. 
.. By changing these parameters, the signal created by the noise()
.. function can be adapted to fit very specific needs and characteristics.

**รูปแบบการใช้งาน**

noiseDetail ( lod, falloff )

**พารามิเตอร์**

- ``lod``  Number: จำนวนเสียงที่จะใช้โดยเสียง

- ``falloff``  Number: falloff factor สำหรับแต่ละ octave

.. ``lod``  Number: number of octaves to be used by the noise
.. ``falloff``  Number: falloff factor for each octave

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	var noiseVal;
	var noiseScale=0.02;
	
	function setup() {
	  createCanvas(100,100);
	}
	
	function draw() {
	  background(0);
	  for (var y = 0; y < height; y++) {
	    for (var x = 0; x < width/2; x++) {
	      noiseDetail(2,0.2);
	      noiseVal = noise((mouseX+x) * noiseScale,
	                       (mouseY+y) * noiseScale);
	      stroke(noiseVal*255);
	      point(x,y);
	      noiseDetail(8,0.65);
	      noiseVal = noise((mouseX + x + width/2) * noiseScale,
	                       (mouseY + y) * noiseScale);
	      stroke(noiseVal*255);
	      point(x + width/2, y);
	    }
	  }
	}

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.

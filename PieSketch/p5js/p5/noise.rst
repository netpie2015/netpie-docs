.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

noise()
=======

ส่งกลับค่าเสียง Perlin ที่พิกัดที่ระบุ เสียง Perlin เป็นเครื่องกำเนิดลำดับแบบสุ่มที่ผลิตลำดับตามลำดับของฮาร์โมนิกที่เป็นธรรมชาติมากขึ้นเมื่อเปรียบเทียบกับฟังก์ชัน random () มาตรฐาน มันถูกคิดค้นโดยเคน Perlin ใน 1980s และถูกใช้ตั้งแต่ในโปรแกรมกราฟิกเพื่อผลิตพื้นผิวขั้นตอนการเคลื่อนไหวธรรมชาติรูปภูมิประเทศ ฯลฯ  ความแตกต่างหลัก ๆ ของฟังก์ชัน random () คือเสียง Perlin ถูกกำหนดไว้ในพื้นที่ n มิติที่ไม่มีที่สิ้นสุดซึ่งคู่พิกัดแต่ละคู่จะสอดคล้องกับค่ากึ่งสุ่มที่คงที่ (คงที่สำหรับอายุการใช้งานของโปรแกรมเท่านั้นดู noiseSeed () ฟังก์ชั่น) p5.js สามารถคำนวณสัญญาณรบกวน 1D, 2D และ 3D ขึ้นอยู่กับจำนวนพิกัดที่กำหนด ค่าที่ได้จะอยู่ระหว่าง 0.0 ถึง 1.0 ค่าเสียงสามารถเคลื่อนไหวได้โดยการเคลื่อนที่ผ่านเนื้อที่เสียงดังที่แสดงในตัวอย่างข้างต้น มิติที่ 2 และ 3 ยังสามารถแปลเป็นเวลา  เสียงจริงมีโครงสร้างคล้ายกับสัญญาณเสียงในส่วนที่เกี่ยวกับการใช้ความถี่ของฟังก์ชัน คล้ายกับแนวคิดของฮาร์โมนิกในฟิสิกส์เสียง perlin จะถูกคำนวณด้วยหลายอ็อกเตฟซึ่งจะรวมกันเพื่อให้ได้ผลลัพธ์สุดท้าย  อีกวิธีหนึ่งในการปรับตัวของลำดับผลลัพธ์คือขนาดของพิกัดอินพุท ในฐานะที่เป็นฟังก์ชันทำงานภายในพื้นที่ที่ไม่มีขีด จำกัด ค่าพิกัดไม่สำคัญเช่นนี้เพียงระยะห่างระหว่างพิกัดที่ต่อเนื่อง (เช่นเมื่อใช้ noise () ภายในลูป) ตามกฎทั่วไปความแตกต่างระหว่างพิกัดจะน้อยลงลำดับเสียงรบกวนที่เกิดขึ้นจะนุ่มนวลขึ้น ขั้นตอนการทำงานของ 0.005-0.03 ให้ผลดีที่สุดสำหรับการใช้งานส่วนใหญ่ แต่จะแตกต่างกันไปขึ้นอยู่กับการใช้งาน

.. Returns the Perlin noise value at specified coordinates. Perlin noise is
.. a random sequence generator producing a more natural ordered, harmonic
.. succession of numbers compared to the standard random() function.
.. It was invented by Ken Perlin in the 1980s and been used since in
.. graphical applications to produce procedural textures, natural motion,
.. shapes, terrains etc. The main difference to the
.. random() function is that Perlin noise is defined in an infinite
.. n-dimensional space where each pair of coordinates corresponds to a
.. fixed semi-random value (fixed only for the lifespan of the program; see
.. the noiseSeed() function). p5.js can compute 1D, 2D and 3D noise,
.. depending on the number of coordinates given. The resulting value will
.. always be between 0.0 and 1.0. The noise value can be animated by moving
.. through the noise space as demonstrated in the example above. The 2nd
.. and 3rd dimension can also be interpreted as time.The actual
.. noise is structured similar to an audio signal, in respect to the
.. function's use of frequencies. Similar to the concept of harmonics in
.. physics, perlin noise is computed over several octaves which are added
.. together for the final result. Another way to adjust the
.. character of the resulting sequence is the scale of the input
.. coordinates. As the function works within an infinite space the value of
.. the coordinates doesn't matter as such, only the distance between
.. successive coordinates does (eg. when using noise() within a
.. loop). As a general rule the smaller the difference between coordinates,
.. the smoother the resulting noise sequence will be. Steps of 0.005-0.03
.. work best for most applications, but this will differ depending on use.

**รูปแบบการใช้งาน**

noise ( x, [y], [z] )

**พารามิเตอร์**

- ``x``  Number: x- ประสานงานในพื้นที่เสียง

- ``y``  Number: y- ประสานงานในพื้นที่เสียง

- ``z``  Number: z - ประสานงานในพื้นที่เสียง

.. ``x``  Number: x-coordinate in noise space
.. ``y``  Number: y-coordinate in noise space
.. ``z``  Number: z-coordinate in noise space

**ค่าที่ส่งออกมา**

- Number: ค่าเสียง Perlin (ระหว่าง 0 ถึง 1) ที่พิกัดที่ระบุ

.. Number: Perlin noise value (between 0 and 1) at specified coordinates

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var xoff = 0.0;
	
	function draw() {
	  background(204);
	  xoff = xoff + .01;
	  var n = noise(xoff) * width;
	  line(n, 0, n, height);
	}

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var noiseScale=0.02;
	
	function draw() {
	  background(0);
	  for (var x=0; x < width; x++) {
	    var noiseVal = noise((mouseX+x)*noiseScale, mouseY*noiseScale);
	    stroke(noiseVal*255);
	    line(x, mouseY+noiseVal*80, x, height);
	  }
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

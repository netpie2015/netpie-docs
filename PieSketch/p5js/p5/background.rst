.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

background()
============

ฟังก์ชัน background () กำหนดสีที่ใช้สำหรับพื้นหลังของ p5.js canvas พื้นหลังดีฟอลต์คือสีเทาอ่อน ใช้ฟังก์ชันนี้ในการวาด () เพื่อล้างหน้าต่างการแสดงผลในตอนเริ่มต้นของแต่ละเฟรม แต่คุณสามารถใช้ภายในการตั้งค่า () เพื่อตั้งค่าพื้นหลังของเฟรมแรกของภาพเคลื่อนไหวหรือหากต้องการตั้งพื้นหลังเพียงครั้งเดียว 
สีระบุเป็นสี RGB, HSB หรือ HSL ขึ้นอยู่กับ colorMode ปัจจุบัน (พื้นที่สีเริ่มต้นคือ RGB โดยแต่ละค่าจะอยู่ในช่วงตั้งแต่ 0 ถึง 255) 
ถ้ามีอาร์กิวเมนต์สตริงเดียวให้ใช้สตริงสี RGB, RGBA และ Hex CSS และสตริงสีที่มีชื่อทั้งหมด ในกรณีนี้ไม่สนับสนุนค่าตัวเลขอัลฟาเป็นอาร์กิวเมนต์ที่สองให้ใช้รูปแบบ RGBA 
วัตถุสี p5. สามารถจัดเตรียมสีพื้นหลังได้เช่นกัน 
p5.Image ยังสามารถให้การตั้งค่าพื้นหลัง iamge

.. The background() function sets the color used for the background of the
.. p5.js canvas. The default background is light gray. This function is
.. typically used within draw() to clear the display window at the beginning
.. of each frame, but it can be used inside setup() to set the background on
.. the first frame of animation or if the background need only be set once.
.. 
.. The color is either specified in terms of the RGB, HSB, or HSL color
.. depending on the current colorMode. (The default color space is RGB, with
.. each value in the range from 0 to 255).
.. 
.. If a single string argument is provided, RGB, RGBA and Hex CSS color strings
.. and all named color strings are supported. In this case, an alpha number
.. value as a second argument is not supported, the RGBA form should be used.
.. 
.. A p5.Color object can also be provided to set the background color.
.. 
.. A p5.Image can also be provided to set the background iamge.

**รูปแบบการใช้งาน**

background ( color, [a] )

**พารามิเตอร์**

- ``color``  p5.Color: ค่าใด ๆ ที่สร้างโดยฟังก์ชัน color ()

- ``a``  Number: ความทึบของพื้นหลังเทียบกับช่วงสีปัจจุบัน (ค่าเริ่มต้นคือ 0-100)

.. ``color``  p5.Color: any value created by the color() function
.. ``a``  Number: opacity of the background relative to current color range (default is 0-100)

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	// Grayscale integer value
	background(51);

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	// R, G & B integer values
	background(255, 204, 0);

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	// H, S & B integer values
	colorMode(HSB);
	background(255, 204, 100);

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	// Named SVG/CSS color string
	background('red');

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	// three-digit hexadecimal RGB notation
	background('#fae');

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	// six-digit hexadecimal RGB notation
	background('#222222');

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	// integer RGB notation
	background('rgb(0,255,0)');

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	// integer RGBA notation
	background('rgba(0,255,0, 0.25)');

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	// percentage RGB notation
	background('rgb(100%,0%,10%)');

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	// percentage RGBA notation
	background('rgba(100%,0%,100%,0.5)');

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	// p5 Color object
	background(color(0, 0, 255));

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

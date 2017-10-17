.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

applyMatrix()
=============

คูณเมทริกซ์ปัจจุบันตามค่าที่กำหนดโดยพารามิเตอร์ นี่คือการดำเนินงานที่มีประสิทธิภาพซึ่งสามารถทำงานได้เทียบเท่ากับการแปล, การวัด, การเฉือนและการหมุนทั้งหมดในครั้งเดียว คุณสามารถเรียนรู้เพิ่มเติมเกี่ยวกับเมทริกซ์การเปลี่ยนแปลงใน วิกิพีเดีย การตั้งชื่อของอาร์กิวเมนต์ที่นี่มีดังต่อไปนี้การตั้งชื่อ ข้อกำหนด WHATWG และสอดคล้องกับเมทริกซ์การเปลี่ยนแปลงของแบบฟอร์ม:> 

.. Multiplies the current matrix by the one specified through the parameters.
.. This is a powerful operation that can perform the equivalent of translate,
.. scale, shear and rotate all at once. You can learn more about transformation
.. matrices on 
.. Wikipedia.
.. The naming of the arguments here follows the naming of the 
.. WHATWG specification and corresponds to a
.. transformation matrix of the
.. form:
.. > 

**รูปแบบการใช้งาน**

applyMatrix ( a, b, c, d, e, f )

**พารามิเตอร์**

- ``a``  Number: ตัวเลขที่กำหนดเมทริกซ์ 2x3 จะคูณ

- ``b``  Number: ตัวเลขที่กำหนดเมทริกซ์ 2x3 จะคูณ

- ``c``  Number: ตัวเลขที่กำหนดเมทริกซ์ 2x3 จะคูณ

- ``d``  Number: ตัวเลขที่กำหนดเมทริกซ์ 2x3 จะคูณ

- ``e``  Number: ตัวเลขที่กำหนดเมทริกซ์ 2x3 จะคูณ

- ``f``  Number: ตัวเลขที่กำหนดเมทริกซ์ 2x3 จะคูณ

.. ``a``  Number: numbers which define the 2x3 matrix to be multiplied
.. ``b``  Number: numbers which define the 2x3 matrix to be multiplied
.. ``c``  Number: numbers which define the 2x3 matrix to be multiplied
.. ``d``  Number: numbers which define the 2x3 matrix to be multiplied
.. ``e``  Number: numbers which define the 2x3 matrix to be multiplied
.. ``f``  Number: numbers which define the 2x3 matrix to be multiplied

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	  frameRate(10);
	  rectMode(CENTER);
	}
	
	function draw() {
	  var step = frameCount % 20;
	  background(200);
	  // Equivalent to translate(x, y);
	  applyMatrix(1, 0, 0, 1, 40 + step, 50);
	  rect(0, 0, 50, 50);
	}

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	  frameRate(10);
	  rectMode(CENTER);
	}
	
	function draw() {
	  var step = frameCount % 20;
	  background(200);
	  translate(50, 50);
	  // Equivalent to scale(x, y);
	  applyMatrix(1 / step, 0, 0, 1 / step, 0, 0);
	  rect(0, 0, 50, 50);
	}

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	  frameRate(10);
	  rectMode(CENTER);
	}
	
	function draw() {
	  var step = frameCount % 20
	  var angle = map(step, 0, 20, 0, TWO_PI);
	  var cos_a = cos(angle);
	  var sin_a = sin(angle);
	  background(200);
	  translate(50, 50);
	  // Equivalent to rotate(angle);
	  applyMatrix(cos_a, sin_a, -sin_a, cos_a, 0, 0);
	  rect(0, 0, 50, 50);
	}

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	  frameRate(10);
	  rectMode(CENTER);
	}
	
	function draw() {
	  var step = frameCount % 20
	  var angle = map(step, 0, 20, -PI/4, PI/4);
	  background(200);
	  translate(50, 50);
	  // equivalent to shearX(angle);
	  var shear_factor = 1 / tan(PI/2 - angle);
	  applyMatrix(1, 0, shear_factor, 1, 0, 0);
	  rect(0, 0, 50, 50);
	}

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.

.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

pointLight()
============

สร้างไฟจุดที่มีสีและตำแหน่งสว่าง

.. Creates a point light with a color and a light position

**รูปแบบการใช้งาน**

pointLight ( v1, [v2], [v3], [a], x, [y], [z] )

**พารามิเตอร์**

- ``v1``  Number,Array,String,p5.Color: ค่าสีเทาค่าสีแดงหรือสี (ขึ้นอยู่กับโหมดสีปัจจุบัน) หรืออาร์เรย์สีหรือสตริงสี CSS

- ``v2``  Number: ตัวเลือก: สีเขียวหรือความอิ่มตัวของสี

- ``v3``  Number: ตัวเลือก: สีน้ำเงินหรือความสว่าง

- ``a``  Number: ตัวเลือก: ความทึบ

- ``x``  Number,p5.Vector: ตำแหน่งแกน x หรือ p5.Vector

- ``y``  Number: ตัวเลือก: ตำแหน่งแกน y

- ``z``  Number: ตำแหน่งแกน z

.. ``v1``  Number,Array,String,p5.Color: gray value, red or hue value (depending on the current color mode), or color Array, or CSS color string
.. ``v2``  Number: optional: green or saturation value
.. ``v3``  Number: optional: blue or brightness value
.. ``a``  Number: optional: opacity
.. ``x``  Number,p5.Vector: x axis position or a p5.Vector
.. ``y``  Number: optional: y axis position
.. ``z``  Number: optional: z axis position

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup(){
	  createCanvas(100, 100, WEBGL);
	}
	function draw(){
	  background(0);
	  //move your mouse to change light position
	  var locY = (mouseY / height - 0.5) *(-2);
	  var locX = (mouseX / width - 0.5) *2;
	  //to set the light position,
	  //think of the world's coordinate as:
	  // -1,1 -------- 1,1
	  //   |            |
	  //   |            |
	  //   |            |
	  // -1,-1---------1,-1
	  pointLight(250, 250, 250, locX, locY, 0);
	  ambientMaterial(250);
	  sphere(50);
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

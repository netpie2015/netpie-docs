.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

perspective()
=============

ตั้งกล้องมุมมอง ค่าที่ตั้งไว้จะเท่ากับมุมมอง (PI / 3.0, width / height, cameraZ / 10.0, cameraZ * 10.0) โดยที่ cameraZ คือ ((สูง / 2.0) / tan (PI * 60.0 / 360.0));

.. Sets perspective camera. When called with no arguments, the defaults
.. provided are equivalent to
.. perspective(PI/3.0, width/height, cameraZ/10.0, cameraZ*10.0)
.. where cameraZ is ((height/2.0) / tan(PI*60.0/360.0));
**รูปแบบการใช้งาน**

perspective ( [fovy], [aspect], [near], [far] )

**พารามิเตอร์**

- ``fovy``  Number: กล้องดูแนวตั้งจากมุมมองด้านล่างถึงมุมมองด้านบนเป็นองศา

- ``aspect``  Number: อัตราสเปรดชีตของกล้อง

- ``near``  Number: frustum ใกล้ระนาบ

- ``far``  Number: frustum ยาวระนาบ

.. ``fovy``  Number: camera frustum vertical field of view,
                          from bottom to top of view, in degrees
.. ``aspect``  Number: camera frustum aspect ratio
.. ``near``  Number: frustum near plane length
.. ``far``  Number: frustum far plane length

**ค่าที่ส่งออกมา**

- p5: วัตถุ p5

.. p5: the p5 object

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	//drag mouse to toggle the world!
	//you will see there's a vanish point
	function setup(){
	  createCanvas(100, 100, WEBGL);
	  var fov = 60 / 180 * PI;
	  var cameraZ = (height/2.0) / tan(fov/2.0);
	  perspective(60 / 180 * PI, width/height, cameraZ * 0.1, cameraZ * 10);
	}
	function draw(){
	 background(200);
	 orbitControl();
	 for(var i = -1; i < 2; i++){
	    for(var j = -2; j < 3; j++){
	      push();
	      translate(i*160, 0, j*160);
	      box(40, 40, 40);
	      pop();
	    }
	  }
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

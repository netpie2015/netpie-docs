.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

plane()
=======

วาดระนาบด้วยความกว้างและความสูง

.. Draw a plane with given a width and height
**รูปแบบการใช้งาน**

plane ( width, height, [detailX], [detailY] )

**พารามิเตอร์**

- ``width``  Number: ความกว้างของเครื่องบิน

- ``height``  Number: ความสูงของเครื่องบิน

- ``detailX``  Number: จำนวนตัวเลือกของสามเหลี่ยมใน x-dimension

- ``detailY``  Number: จำนวนตัวอยางของสวนยอยสามเหลี่ยมใน y-dimension

.. ``width``  Number: width of the plane
.. ``height``  Number: height of the plane
.. ``detailX``  Number: Optional number of triangle
                            subdivisions in x-dimension
.. ``detailY``  Number: Optional number of triangle
                            subdivisions in y-dimension

**ค่าที่ส่งออกมา**

- p5: วัตถุ p5

.. p5: the p5 object

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	//draw a plane with width 200 and height 200
	function setup(){
	  createCanvas(100, 100, WEBGL);
	}
	
	function draw(){
	  background(200);
	  plane(50, 50);
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

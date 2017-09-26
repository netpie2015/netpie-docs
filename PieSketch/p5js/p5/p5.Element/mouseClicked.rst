.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

mouseClicked()
==============

ฟังก์ชัน mousesClicked () เรียกว่าครั้งหลังจากที่กดปุ่มเมาส์และปล่อยผ่านองค์ประกอบ สามารถใช้เพื่อแนบผู้ฟังเหตุการณ์เฉพาะบางส่วน

.. The .mouseClicked() function is called once after a mouse button is
.. pressed and released over the element. This can be used to
.. attach element specific event listeners.

**รูปแบบการใช้งาน**

mouseClicked ( fxn )

**พารามิเตอร์**

- ``fxn``  function: ฟังก์ชั่นที่จะยิงเมื่อมีการคลิกเมาส์เหนือองค์ประกอบ

.. ``fxn``  function: function to be fired when mouse is clicked over the element.

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var cnv;
	var d;
	var g;
	
	function setup() {
	  cnv = createCanvas(100, 100);
	  cnv.mouseClicked(changeGray); // attach listener for
	                                // activity on canvas only
	  d = 10;
	  g = 100;
	}
	
	function draw() {
	  background(g);
	  ellipse(width/2, height/2, d, d);
	}
	
	// this function fires after the mouse has been
	// clicked anywhere
	function mouseClicked() {
	  d = d + 10;
	}
	
	// this function fires after the mouse has been
	// clicked on canvas
	function changeGray() {
	  g = random(0, 255);
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

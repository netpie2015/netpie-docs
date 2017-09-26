.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

mousePressed()
==============

ฟังก์ชัน. mousePressed () เรียกว่าครั้งหลังจากทุกครั้งที่กดปุ่มเมาส์เหนือองค์ประกอบ สามารถใช้เพื่อแนบผู้ฟังเหตุการณ์เฉพาะบางส่วน

.. The .mousePressed() function is called once after every time a
.. mouse button is pressed over the element. This can be used to
.. attach element specific event listeners.
**รูปแบบการใช้งาน**

mousePressed ( fxn )

**พารามิเตอร์**

- ``fxn``  function: ฟังก์ชั่นที่จะยิงเมื่อเมาส์ถูกกดเหนือองค์ประกอบ

.. ``fxn``  function: function to be fired when mouse is
                   pressed over the element.

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var cnv;
	var d;
	var g;
	function setup() {
	  cnv = createCanvas(100, 100);
	  cnv.mousePressed(changeGray); // attach listener for
	                                // canvas click only
	  d = 10;
	  g = 100;
	}
	
	function draw() {
	  background(g);
	  ellipse(width/2, height/2, d, d);
	}
	
	// this function fires with any click anywhere
	function mousePressed() {
	  d = d + 10;
	}
	
	// this function fires only when cnv is clicked
	function changeGray() {
	  g = random(0, 255);
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

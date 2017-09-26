.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

doubleClicked()
===============

ฟังก์ชัน doubleClicked () เรียกว่าครั้งหลังจากทุกครั้งที่กดปุ่มเมาส์สองครั้งเหนือองค์ประกอบ ซึ่งสามารถใช้เพื่อแนบผู้ฟังเหตุการณ์ของ element และ action ได้

.. The .doubleClicked() function is called once after every time a
.. mouse button is pressed twice over the element. This can be used to
.. attach element and action specific event listeners.

**รูปแบบการใช้งาน**

doubleClicked ( fxn )

**พารามิเตอร์**

- ``fxn``  function: ฟังก์ชั่นที่จะยิงเมื่อเมาส์ถูกกดเหนือองค์ประกอบ

.. ``fxn``  function: function to be fired when mouse is pressed over the element.

**ค่าที่ส่งออกมา**

- p5.Element: 

.. p5.Element: 

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var cnv;
	var d;
	var g;
	function setup() {
	  cnv = createCanvas(100, 100);
	  cnv.doubleClicked(changeGray); // attach listener for
	                                // canvas click only
	  d = 10;
	  g = 100;
	}
	
	function draw() {
	  background(g);
	  ellipse(width/2, height/2, d, d);
	}
	
	// this function fires with any double click anywhere
	function doubleClicked() {
	  d = d + 10;
	}
	
	// this function fires only when cnv is clicked
	function changeGray() {
	  g = random(0, 255);
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

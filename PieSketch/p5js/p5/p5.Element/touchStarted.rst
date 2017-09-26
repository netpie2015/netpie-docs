.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

touchStarted()
==============

ฟังก์ชัน touchStarted () เรียกว่าครั้งหลังจากลงทะเบียนแล้วทุกครั้ง สามารถใช้เพื่อแนบผู้ฟังเหตุการณ์เฉพาะบางส่วน

.. The .touchStarted() function is called once after every time a touch is
.. registered. This can be used to attach element specific event listeners.

**รูปแบบการใช้งาน**

touchStarted ( fxn )

**พารามิเตอร์**

- ``fxn``  function: ฟังก์ชันที่จะถูกเรียกใช้เมื่อเริ่มต้นสัมผัสกับองค์ประกอบ

.. ``fxn``  function: function to be fired when touch is started over the element.

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var cnv;
	var d;
	var g;
	function setup() {
	  cnv = createCanvas(100, 100);
	  cnv.touchStarted(changeGray); // attach listener for
	                                // canvas click only
	  d = 10;
	  g = 100;
	}
	
	function draw() {
	  background(g);
	  ellipse(width/2, height/2, d, d);
	}
	
	// this function fires with any touch anywhere
	function touchStarted() {
	  d = d + 10;
	}
	
	// this function fires only when cnv is clicked
	function changeGray() {
	  g = random(0, 255);
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

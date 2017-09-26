.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

mouseOver()
===========

ฟังก์ชัน. mouseOver () เรียกว่าครั้งหลังจากที่เมาส์เคลื่อนที่ไปยังองค์ประกอบทุกครั้ง สามารถใช้เพื่อแนบผู้ฟังเหตุการณ์เฉพาะบางส่วน

.. The .mouseOver() function is called once after every time a
.. mouse moves onto the element. This can be used to attach an
.. element specific event listener.
**รูปแบบการใช้งาน**

mouseOver ( fxn )

**พารามิเตอร์**

- ``fxn``  function: ฟังก์ชั่นที่จะยิงเมื่อเมาส์ถูกย้ายไปยังองค์ประกอบ

.. ``fxn``  function: function to be fired when mouse is
                   moved over the element.

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var cnv;
	var d;
	var g;
	function setup() {
	  cnv = createCanvas(100, 100);
	  cnv.mouseOver(changeGray);
	  d = 10;
	}
	
	function draw() {
	  ellipse(width/2, height/2, d, d);
	}
	
	function changeGray() {
	  d = d + 10;
	  if (d > 100) {
	    d = 0;
	  }
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

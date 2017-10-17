.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

mouseWheel()
============

ฟังก์ชัน. mouseWheel () เรียกว่าครั้งหลังจากทุกครั้งที่มีการเลื่อนเมาส์ไปบนองค์ประกอบ สามารถใช้เพื่อแนบผู้ฟังเหตุการณ์เฉพาะบางส่วน 
ฟังก์ชันรับฟังก์ชันเรียกกลับเป็นอาร์กิวเมนต์ซึ่งจะทำงานเมื่อเหตุการณ์ `ล้อเลื่อนถูกเรียกใช้บนองค์ประกอบฟังก์ชันการเรียกกลับจะถูกส่งผ่านเหตุการณ์` อาร์กิวเมนต์หนึ่ง ๆ ' คุณสมบัติ `event.deltaY` ส่งกลับค่าลบหากล้อเลื่อนของเมาส์ถูกหมุนขึ้นหรือออกจากผู้ใช้และบวกในทิศทางอื่น `event.deltaX` ทำเช่นเดียวกับ` event.deltaY` ยกเว้นจะอ่านสเกลล้อแนวนอนของล้อเลื่อนเมาส์ 
ใน OS X ที่มีการเลื่อนแบบ "ธรรมชาติ" ค่าของ event.local จะกลับรายการ

.. The .mouseWheel() function is called once after every time a
.. mouse wheel is scrolled over the element. This can be used to
.. attach element specific event listeners.
.. 
.. The function accepts a callback function as argument which will be executed
.. when the `wheel` event is triggered on the element, the callback function is
.. passed one argument `event`. The `event.deltaY` property returns negative
.. values if the mouse wheel is rotated up or away from the user and positive
.. in the other direction. The `event.deltaX` does the same as `event.deltaY`
.. except it reads the horizontal wheel scroll of the mouse wheel.
.. 
.. On OS X with "natural" scrolling enabled, the `event.deltaY` values are
.. reversed.

**รูปแบบการใช้งาน**

mouseWheel ( fxn )

**พารามิเตอร์**

- ``fxn``  function: จะถูกเรียกใช้เมื่อเลื่อนเมาส์ไปบนองค์ประกอบ

.. ``fxn``  function: function to be fired when mouse wheel is scrolled over the element.

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var cnv;
	var d;
	var g;
	function setup() {
	  cnv = createCanvas(100, 100);
	  cnv.mouseWheel(changeSize); // attach listener for
	                              // activity on canvas only
	  d = 10;
	  g = 100;
	}
	
	function draw() {
	  background(g);
	  ellipse(width/2, height/2, d, d);
	}
	
	// this function fires with mousewheel movement
	// anywhere on screen
	function mouseWheel() {
	  g = g + 10;
	}
	
	// this function fires with mousewheel movement
	// over canvas only
	function changeSize(event) {
	  if (event.deltaY > 0) {
	    d = d + 10;
	  } else {
	    d = d - 10;
	  }
	}

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.

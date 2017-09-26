.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

dragOver()
==========

ฟังก์ชัน. dragOver () เรียกว่าครั้งหลังจากที่มีการลากไฟล์ไปยังองค์ประกอบทุกครั้ง สามารถใช้เพื่อแนบผู้ฟังเหตุการณ์เฉพาะบางส่วน

.. The .dragOver() function is called once after every time a
.. file is dragged over the element. This can be used to attach an
.. element specific event listener.
**รูปแบบการใช้งาน**

dragOver ( fxn )

**พารามิเตอร์**

- ``fxn``  function: จะถูกเรียกใช้เมื่อลากเมาส์ไปเหนือองค์ประกอบ

.. ``fxn``  function: function to be fired when mouse is
                   dragged over the element.

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	// To test this sketch, simply drag a
	// file over the canvas
	function setup() {
	  var c = createCanvas(100, 100);
	  background(200);
	  textAlign(CENTER);
	  text('Drag file', width/2, height/2);
	  c.dragOver(dragOverCallback);
	}
	
	// This function will be called whenever
	// a file is dragged over the canvas
	function dragOverCallback() {
	  background(240);
	  text('Dragged over', width/2, height/2);
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

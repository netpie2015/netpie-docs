.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

curveTightness()
================

ปรับเปลี่ยนคุณภาพของฟอร์มที่สร้างด้วยเส้นโค้ง () และ curveVertex () ความหนาแน่นของพารามิเตอร์กำหนดว่าเส้นโค้งจะพอดีกับจุดยอดจุดไหน ค่านี้เป็นค่าดีฟอลต์สำหรับความรัดกุม (ค่านี้กำหนดเส้นโค้งให้เป็นรูปทรงกระบอก Catmull-Rom) และค่า 1.0 จะเชื่อมต่อจุดทั้งหมดด้วยเส้นตรง ค่าในช่วง -5.0 และ 5.0 จะเปลี่ยนรูปโค้ง แต่จะทำให้พวกเขาเป็นที่รู้จักและเป็นค่าที่เพิ่มขึ้นในขนาดที่พวกเขาจะยังคงทำให้เสียโฉม

.. Modifies the quality of forms created with curve() and curveVertex().
.. The parameter tightness determines how the curve fits to the vertex
.. points. The value 0.0 is the default value for tightness (this value
.. defines the curves to be Catmull-Rom splines) and the value 1.0 connects
.. all the points with straight lines. Values within the range -5.0 and 5.0
.. will deform the curves but will leave them recognizable and as values
.. increase in magnitude, they will continue to deform.
**รูปแบบการใช้งาน**

curveTightness ( amount )

**พารามิเตอร์**

- ``amount``  Number: ของการเปลี่ยนรูปจากจุดยอดเดิม

.. ``amount``  Number: of deformation from the original vertices

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	// Move the mouse left and right to see the curve change
	
	function setup() {
	  createCanvas(100, 100);
	  noFill();
	}
	
	function draw() {
	  background(204);
	  var t = map(mouseX, 0, width, -5, 5);
	  curveTightness(t);
	  beginShape();
	  curveVertex(10, 26);
	  curveVertex(10, 26);
	  curveVertex(83, 24);
	  curveVertex(83, 61);
	  curveVertex(25, 65);
	  curveVertex(25, 65);
	  endShape();
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

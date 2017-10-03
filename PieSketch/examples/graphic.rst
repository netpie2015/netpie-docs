.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

การวาดภาพกราฟฟิก
================

การวาดภาพกราฟฟิกด้วย p5.js และเคลื่อนที่ตามตำแหน่งลูกศรของเมาส์ที่ลากไปมาบนบริเวณของพื้นที่กรอบสีเหลี่ยม

อ้างอิง: https://p5js.org/examples/structure-create-graphics.html

.. raw:: html

	<script type="text/p5" data-height="400" data-preview-width="400">
	function setup(){
		createCanvas(400, 320);
	}

	function draw(){
		fill(0, 12);
		rect(0, 0, width, height);
		fill(255);
		noStroke();
		ellipse(mouseX, mouseY, 60, 60);
	}
	</script>
	<p></p>

.. toctree::
	:hidden:

	การวาดภาพกราฟฟิก <examples/graphic>
	การควบคุมเปลี่ยนแปลงสี <examples/control_rgb>
	ภาพเคลี่อนไหว 2D <examples/2d>
	ภาพเคลี่อนไหว 3D <examples/3d>
	การสื่อสารระหว่าง p5.js ผ่าน NETPIE <examples/microgear>



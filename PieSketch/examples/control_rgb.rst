.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

การควบคุมเปลี่ยนแปลงสี
====================

การแปลี่ยนแปลงสีพื้นหลังตามค่าสี RGB ที่กำหนด โดยการปรับค่าบน Slider

อ้างอิง: https://p5js.org/examples/dom-slider.html

.. raw:: html

	<script type="text/p5" data-height="400" data-preview-width="400">
	var rSlider, gSlider, bSlider;

	function setup() {
		// create canvas
		createCanvas(400, 320);
		textSize(15);
		noStroke();

		// create sliders
		rSlider = createSlider(0, 255, 100);
		rSlider.position(20, 20);
		gSlider = createSlider(0, 255, 0);
		gSlider.position(20, 50);
		bSlider = createSlider(0, 255, 255);
		bSlider.position(20, 80);
	}

	function draw() {
		var r = rSlider.value();
		var g = gSlider.value();
		var b = bSlider.value();
		background(r, g, b);
		text("red", rSlider.x * 2 + rSlider.width, 35);
		text("green", gSlider.x * 2 + gSlider.width, 65);
		text("blue", bSlider.x * 2 + bSlider.width, 95);
	}
	</script>
	<p></p>

.. toctree::
	:hidden:

	การวาดภาพกราฟฟิก <examples/graphic>
	การควบคุมเปลี่ยนแปลงสี <examples/control_rgb>
	ภาพเคลี่อนไหว 2D <examples/2d>
	ภาพเคลี่อนไหว 3D <examples/3d>
	การสื่อสารระหว่าง Alice กับ Bob ผ่าน NETPIE <examples/microgear>



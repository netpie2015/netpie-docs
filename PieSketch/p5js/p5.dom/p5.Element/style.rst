.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

style()
=======

ตั้งค่าคุณสมบัติสไตล์ (css) ที่ระบุ (อาร์กิวเมนต์ที่ 1) ขององค์ประกอบด้วยค่าที่กำหนด (อาร์เรย์ที่ 2) ถ้าอาร์กิวเมนต์เดียวถูกกำหนดให้. style () ส่งกลับค่าของคุณสมบัติที่ระบุ แต่ถ้าอาร์กิวเมนต์เดียวถูกกำหนดในรูปแบบ CSS ('text-align: center'), .style () จะตั้งค่า CSS ให้เหมาะสม รูปแบบ. () ยังจัดการ 2D และ 3D css transforms ถ้า arg ที่ 1 คือ 'หมุน', 'แปล' หรือ 'ตำแหน่ง' อาร์กิวเมนต์ต่อไปนี้จะยอมรับตัวเลขเป็นค่า ('แปล', 10, 100, 50);

.. Sets the given style (css) property (1st arg) of the element with the
.. given value (2nd arg). If a single argument is given, .style()
.. returns the value of the given property; however, if the single argument
.. is given in css syntax ('text-align:center'), .style() sets the css
.. appropriatly. .style() also handles 2d and 3d css transforms. If
.. the 1st arg is 'rotate', 'translate', or 'position', the following arguments
.. accept Numbers as values. ('translate', 10, 100, 50);

**รูปแบบการใช้งาน**

style ( property, [value] )

**พารามิเตอร์**

- ``property``  String: คุณสมบัติที่จะตั้งค่า

- ``value``  String,Number,p5.Color: ค่าที่จะกำหนดให้กับคุณสมบัติ (เฉพาะสตริง | จำนวนสำหรับหมุน / แปล)

.. ``property``  String: property to be set
.. ``value``  String,Number,p5.Color: value to assign to property (only String|Number for rotate/translate)

**ค่าที่ส่งออกมา**

- String,Object,p5.Element: ค่าของคุณสมบัติถ้าไม่มีค่าระบุหรือ p5.Element

.. String,Object,p5.Element: value of property, if no value is specified or p5.Element

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	<code class="norender">
	var myDiv = createDiv("I like pandas.");
	myDiv.style("font-size", "18px");
	myDiv.style("color", "#ff0000");
	<code class="norender">
	var col = color(25,23,200,50);
	var button = createButton("button");
	button.style("background-color", col);
	button.position(10, 10);
	<code class="norender">
	var myDiv = createDiv("I like lizards.");
	myDiv.style("position", 20, 20);
	myDiv.style("rotate", 45);
	<code class="norender">
	var myDiv;
	function setup() {
	  background(200);
	  myDiv = createDiv("I like gray.");
	  myDiv.position(20, 20);
	}
	
	function draw() {
	  myDiv.style("font-size", mouseX+"px");
	}

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.

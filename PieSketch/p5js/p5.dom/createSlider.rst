.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

createSlider()
==============

สร้างตัวเลื่อน   องค์ประกอบใน DOM ใช้. size () เพื่อตั้งค่าความยาวของแถบเลื่อน ผนวกเข้ากับโหนดคอนเทนเนอร์หากมีการระบุไว้มิฉะนั้นจะต่อท้ายกับเนื้อหา

.. Creates a slider &lt;input&gt;&lt;/input&gt; element in the DOM.
.. Use .size() to set the display length of the slider.
.. Appends to the container node if one is specified, otherwise
.. appends to body.

**รูปแบบการใช้งาน**

createSlider ( min, max, [value], [step] )

**พารามิเตอร์**

- ``min``  Number: ค่าต่ำสุดของแถบเลื่อน

- ``max``  Number: ค่าสูงสุดของแถบเลื่อน

- ``value``  Number: ค่าเริ่มต้นของแถบเลื่อน

- ``step``  Number: (ถ้าขั้นตอนตั้งค่าเป็น 0 แถบเลื่อนจะเคลื่อนที่อย่างต่อเนื่องจากค่าต่ำสุดถึงสูงสุด)

.. ``min``  Number: minimum value of the slider
.. ``max``  Number: maximum value of the slider
.. ``value``  Number: default value of the slider
.. ``step``  Number: step size for each tick of the slider (if step is set to 0, the slider will move continuously from the minimum to the maximum value)

**ค่าที่ส่งออกมา**

- Object,p5.Element: ชี้ไปที่ p5.Element ถือสร้างโหนด

.. Object,p5.Element: pointer to p5.Element holding created node

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var slider;
	function setup() {
	  slider = createSlider(0, 255, 100);
	  slider.position(10, 10);
	  slider.style('width', '80px');
	}
	
	function draw() {
	  var val = slider.value();
	  background(val);
	}
	var slider;
	function setup() {
	  colorMode(HSB);
	  slider = createSlider(0, 360, 60, 40);
	  slider.position(10, 10);
	  slider.style('width', '80px');
	}
	
	function draw() {
	  var val = slider.value();
	  background(val, 100, 100, 1);
	}

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.

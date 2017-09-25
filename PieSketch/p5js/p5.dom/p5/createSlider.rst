.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

createSlider()
==============

Creates a slider &lt;input&gt;&lt;/input&gt; element in the DOM.
Use .size() to set the display length of the slider.
Appends to the container node if one is specified, otherwise
appends to body.

**รูปแบบการใช้งาน**

createSlider ( min, max, [value], [step] )

**พารามิเตอร์**

- ``min``  Number: minimum value of the slider

- ``max``  Number: maximum value of the slider

- ``value``  Number: default value of the slider

- ``step``  Number: step size for each tick of the slider (if step is set to 0, the slider will move continuously from the minimum to the maximum value)


**ค่าที่ส่งออกมา**

- Object,p5.Element: pointer to p5.Element holding created node


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

.. toctree::


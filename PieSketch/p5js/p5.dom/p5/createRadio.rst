.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

createRadio()
=============

Creates a radio button &lt;input&gt;&lt;/input&gt; element in the DOM.
The .option() method can be used to set options for the radio after it is
created. The .value() method will return the currently selected option.

**รูปแบบการใช้งาน**

createRadio ( [divId] )

**พารามิเตอร์**

- ``divId``  String: the id and name of the created div and input field respectively


**ค่าที่ส่งออกมา**

- Object,p5.Element: pointer to p5.Element holding created node


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var radio;
	
	function setup() {
	  radio = createRadio();
	  radio.option("black");
	  radio.option("white");
	  radio.option("gray");
	  radio.style('width', '60px');
	  textAlign(CENTER);
	  fill(255, 0, 0);
	}
	
	function draw() {
	  var val = radio.value();
	  background(val);
	  text(val, width/2, height/2);
	}
	var radio;
	
	function setup() {
	  radio = createRadio();
	  radio.option('apple', 1);
	  radio.option('bread', 2);
	  radio.option('juice', 3);
	  radio.style('width', '60px');
	  textAlign(CENTER);
	}
	
	function draw() {
	  background(200);
	  var val = radio.value();
	  if (val) {
	    text('item cost is $'+val, width/2, height/2);
	  }
	}

	</script>

	<br><br>

.. toctree::


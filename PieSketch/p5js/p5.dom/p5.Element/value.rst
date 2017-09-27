.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

value()
=======

ทั้งส่งกลับค่าขององค์ประกอบถ้าอาร์กิวเมนต์ไม่ได้รับหรือกำหนดค่าขององค์ประกอบ

.. Either returns the value of the element if no arguments
.. given, or sets the value of the element.

**รูปแบบการใช้งาน**

value ( [value] )

**พารามิเตอร์**

- ``value``  String,Number: 

.. ``value``  String,Number: 

**ค่าที่ส่งออกมา**

- String,Object,p5.Element: ค่าขององค์ประกอบถ้าไม่มีการระบุค่าหรือ p5.Element

.. String,Object,p5.Element: value of element if no value is specified or p5.Element

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	// gets the value
	var inp;
	function setup() {
	  inp = createInput('');
	}
	
	function mousePressed() {
	  print(inp.value());
	}
	// sets the value
	var inp;
	function setup() {
	  inp = createInput('myValue');
	}
	
	function mousePressed() {
	  inp.value("myValue");
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

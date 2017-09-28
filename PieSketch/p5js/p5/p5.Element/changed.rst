.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

changed()
=========

ฟังก์ชัน .changed () จะถูกเรียกเมื่อเปลี่ยนค่าขององค์ประกอบ สามารถใช้เพื่อแนบผู้ฟังเหตุการณ์เฉพาะบางส่วน

.. The .changed() function is called when the value of an
.. element is changed.
.. This can be used to attach an element specific event listener.

**รูปแบบการใช้งาน**

changed ( fxn )

**พารามิเตอร์**

- ``fxn``  function: จะถูกเรียกใช้เมื่อค่าขององค์ประกอบเปลี่ยนแปลง

.. ``fxn``  function: function to be fired when the value of an element changes.

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var sel;
	
	function setup() {
	  textAlign(CENTER);
	  background(200);
	  sel = createSelect();
	  sel.position(10, 10);
	  sel.option('pear');
	  sel.option('kiwi');
	  sel.option('grape');
	  sel.changed(mySelectEvent);
	}
	
	function mySelectEvent() {
	  var item = sel.value();
	  background(200);
	  text("it's a "+item+"!", 50, 50);
	}
	var checkbox;
	var cnv;
	
	function setup() {
	  checkbox = createCheckbox(" fill");
	  checkbox.changed(changeFill);
	  cnv = createCanvas(100, 100);
	  cnv.position(0, 30);
	  noFill();
	}
	
	function draw() {
	  background(200);
	  ellipse(50, 50, 50, 50);
	}
	
	function changeFill() {
	  if (checkbox.checked()) {
	    fill(0);
	  } else {
	    noFill();
	  }
	}

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.

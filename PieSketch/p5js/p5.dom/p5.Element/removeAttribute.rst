.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

removeAttribute()
=================

Removes an attribute on the specified element.

**รูปแบบการใช้งาน**

removeAttribute ( attr )

**พารามิเตอร์**

- ``attr``  String: attribute to remove


**ค่าที่ส่งออกมา**

- Object,p5.Element: 


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var button;
	var checkbox;
	
	function setup() {
	  checkbox = createCheckbox('enable', true);
	  checkbox.changed(enableButton);
	  button = createButton('button');
	  button.position(10, 10);
	}
	
	function enableButton() {
	  if( this.checked() ) {
	    // Re-enable the button
	    button.removeAttribute('disabled');
	  } else {
	    // Disable the button
	    button.attribute('disabled','');
	  }
	}

	</script>

	<br><br>

.. toctree::


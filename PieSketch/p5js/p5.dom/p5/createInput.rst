.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

createInput()
=============

Creates an &lt;input&gt;&lt;/input&gt; element in the DOM for text input.
Use .size() to set the display length of the box.
Appends to the container node if one is specified, otherwise
appends to body.

**รูปแบบการใช้งาน**

createInput ( [value], [type] )

**พารามิเตอร์**

- ``value``  Number: default value of the input box

- ``type``  String: type of text, ie text, password etc. Defaults to text


**ค่าที่ส่งออกมา**

- Object,p5.Element: pointer to p5.Element holding created node


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup(){
	  var inp = createInput('');
	  inp.input(myInputEvent);
	}
	
	function myInputEvent(){
	  console.log('you are typing: ', this.value());
	}
	

	</script>

	<br><br>

.. toctree::


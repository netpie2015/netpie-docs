.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

input()
=======

The .input() function is called when any user input is
detected with an element. The input event is often used
to detect keystrokes in a input element, or changes on a
slider element. This can be used to attach an element specific
event listener.

**รูปแบบการใช้งาน**

input ( fxn )

**พารามิเตอร์**

- ``fxn``  function: function to be fired on user input.


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	// Open your console to see the output
	function setup() {
	  var inp = createInput('');
	  inp.input(myInputEvent);
	}
	
	function myInputEvent() {
	  console.log('you are typing: ', this.value());
	}

	</script>

	<br><br>

.. toctree::


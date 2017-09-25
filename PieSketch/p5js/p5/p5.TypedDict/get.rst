.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

get()
=====

Returns value stored at supplied key.

**รูปแบบการใช้งาน**

get ( key )

**พารามิเตอร์**

- ``key``  Number,String: that you want to access


**ค่าที่ส่งออกมา**

- Number,String: the value stored at that key


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	function setup() {
	  var myDictionary = createStringDict('p5', 'js');
	  var myValue = myDictionary.get('p5');
	  print(myValue === 'js'); // logs true to console
	}
	

	</script>

	<br><br>

.. toctree::


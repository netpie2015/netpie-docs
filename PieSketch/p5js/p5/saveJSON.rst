.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

saveJSON()
==========

Writes the contents of an Array or a JSON object to a .json file.
 The file saving process and location of the saved file will
 vary between web browsers.

**รูปแบบการใช้งาน**

saveJSON ( json, filename, [optimize] )

**พารามิเตอร์**

- ``json``  Array,Object: 

- ``filename``  String: 

- ``optimize``  Boolean: If true, removes line breaks and spaces from the output file to optimize filesize (but not readability).


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	 var json;
	
	 function setup() {
	
	   json = {}; // new JSON Object
	
	   json.id = 0;
	   json.species = 'Panthera leo';
	   json.name = 'Lion';
	
	 // To save, un-comment the line below, then click 'run'
	 // saveJSON(json, 'lion.json');
	 }
	
	 // Saves the following to a file called "lion.json":
	 // {
	 //   "id": 0,
	 //   "species": "Panthera leo",
	 //   "name": "Lion"
	 // }
	 

	</script>

	<br><br>

.. toctree::


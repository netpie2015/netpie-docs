.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

getRow()
========

Returns a reference to the specified p5.TableRow. The reference
can then be used to get and set values of the selected row.

**รูปแบบการใช้งาน**

getRow ( rowID )

**พารามิเตอร์**

- ``rowID``  : ID number of the row to get


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	// Given the CSV file "mammals.csv"
	// in the project's "assets" folder:
	//
	// id,species,name
	// 0,Capra hircus,Goat
	// 1,Panthera pardus,Leopard
	// 2,Equus zebra,Zebra
	
	var table;
	
	function preload() {
	  //my table is comma separated value "csv"
	  //and has a header specifying the columns labels
	  table = loadTable("assets/mammals.csv", "csv", "header");
	}
	
	function setup() {
	  var row = table.getRow(1);
	  //print it column by column
	  //note: a row is an object, not an array
	  for (var c = 0; c < table.getColumnCount(); c++)
	    print(row.getString(c));
	}
	</script>

	<br><br>

.. toctree::


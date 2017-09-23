.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

addRow()
========

Use addRow() to add a new row of data to a p5.Table object. By default,
 an empty row is created. Typically, you would store a reference to
 the new row in a TableRow object (see newRow in the example above),
 and then set individual values using set().
 If a p5.TableRow object is included as a parameter, then that row is
 duplicated and added to the table.

**รูปแบบการใช้งาน**

addRow ( [row] )

**พารามิเตอร์**

- ``row``  : row to be added to the table


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
	  //add a row
	  var newRow = table.addRow();
	  newRow.setString("id", table.getRowCount() - 1);
	  newRow.setString("species", "Canis Lupus");
	  newRow.setString("name", "Wolf");
	
	  //print the results
	  for (var r = 0; r < table.getRowCount(); r++)
	    for (var c = 0; c < table.getColumnCount(); c++)
	      print(table.getString(r, c));
	}
	</script>

	<br><br>

.. toctree::


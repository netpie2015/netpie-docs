.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

addColumn()
===========

Use addColumn() to add a new column to a Table object.
 Typically, you will want to specify a title, so the column
 may be easily referenced later by name. (If no title is
 specified, the new column's title will be null.)

**รูปแบบการใช้งาน**

addColumn ( [title] )

**พารามิเตอร์**

- ``title``  String: title of the given column


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
	  table.addColumn("carnivore");
	  table.set(0, "carnivore", "no");
	  table.set(1, "carnivore", "yes");
	  table.set(2, "carnivore", "no");
	
	  //print the results
	  for (var r = 0; r < table.getRowCount(); r++)
	    for (var c = 0; c < table.getColumnCount(); c++)
	      print(table.getString(r, c));
	}

	</script>

	<br><br>

.. toctree::


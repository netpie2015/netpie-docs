.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

findRows()
==========

Finds the rows in the Table that contain the value
 provided, and returns references to those rows. Returns an
 Array, so for must be used to iterate through all the rows,
 as shown in the example above. The column to search may be
 specified by either its ID or title.

**รูปแบบการใช้งาน**

findRows ( value, column )

**พารามิเตอร์**

- ``value``  String: The value to match

- ``column``  Number,String: ID number or title of the column to search


**ค่าที่ส่งออกมา**

- Array.<p5.TableRow>: An Array of TableRow objects


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
	  //add another goat
	  var newRow = table.addRow();
	  newRow.setString("id", table.getRowCount() - 1);
	  newRow.setString("species", "Scape Goat");
	  newRow.setString("name", "Goat");
	
	  //find the rows containing animals named Goat
	  var rows = table.findRows("Goat", "name");
	  print(rows.length + " Goats found");
	}

	</script>

	<br><br>

.. toctree::


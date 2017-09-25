.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

getColumn()
===========

Retrieves all values in the specified column, and returns them
 as an array. The column may be specified by either its ID or title.

**รูปแบบการใช้งาน**

getColumn ( column )

**พารามิเตอร์**

- ``column``  String,Number: String or Number of the column to return


**ค่าที่ส่งออกมา**

- Array: Array of column values


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
	  //getColumn returns an array that can be printed directly
	  print(table.getColumn("species"));
	  //outputs ["Capra hircus", "Panthera pardus", "Equus zebra"]
	}

	</script>

	<br><br>

.. toctree::


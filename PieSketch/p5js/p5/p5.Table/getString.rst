.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

getString()
===========

Retrieves a String value from the Table's specified row and column.
The row is specified by its ID, while the column may be specified by
either its ID or title.

**รูปแบบการใช้งาน**

getString ( row, column )

**พารามิเตอร์**

- ``row``  Number: row ID

- ``column``  String,Number: columnName (string) or ID (number)


**ค่าที่ส่งออกมา**

- String: 


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
	  var tableArray = table.getArray();
	
	  //output each row as array
	  for (var i = 0; i < tableArray.length; i++)
	    print(tableArray[i]);
	}

	</script>

	<br><br>

.. toctree::


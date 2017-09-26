.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

removeRow()
===========

ลบแถวออกจากวัตถุตาราง

.. Removes a row from the table object.
**รูปแบบการใช้งาน**

removeRow ( id )

**พารามิเตอร์**

- ``id``  Number: หมายเลขประจำตัวของแถวที่จะลบ

.. ``id``  Number: ID number of the row to remove

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
	  //remove the first row
	  var r = table.removeRow(0);
	
	  //print the results
	  for (var r = 0; r < table.getRowCount(); r++)
	    for (var c = 0; c < table.getColumnCount(); c++)
	      print(table.getString(r, c));
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

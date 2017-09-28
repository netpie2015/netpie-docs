.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

clearRows()
===========

ลบแถวทั้งหมดออกจากตาราง แม้ว่าแถวทั้งหมดจะถูกลบออกคอลัมน์และชื่อคอลัมน์จะยังคงอยู่

.. Removes all rows from a Table. While all rows are removed,
..  columns and column titles are maintained.

**รูปแบบการใช้งาน**

clearRows ( )

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
	  table.clearRows();
	  print(table.getRowCount() + " total rows in table");
	  print(table.getColumnCount() + " total columns in table");
	}

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.

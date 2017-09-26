.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

removeColumn()
==============

ใช้ removeColumn () เพื่อลบคอลัมน์ที่มีอยู่ออกจากอ็อบเจ็กต์ Table คอลัมน์ที่จะลบอาจถูกระบุด้วยชื่อ (สตริง) หรือค่าดัชนี (int) removeColumn (0) จะลบคอลัมน์แรก removeColumn (1) จะลบคอลัมน์ที่สองและอื่น ๆ

.. Use removeColumn() to remove an existing column from a Table
..  object. The column to be removed may be identified by either
..  its title (a String) or its index value (an int).
..  removeColumn(0) would remove the first column, removeColumn(1)
..  would remove the second column, and so on.

**รูปแบบการใช้งาน**

removeColumn ( column )

**พารามิเตอร์**

- ``column``  String,Number: columnName (string) หรือ ID (number)

.. ``column``  String,Number: columnName (string) or ID (number)

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
	  table.removeColumn("id");
	  print(table.getColumnCount());
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

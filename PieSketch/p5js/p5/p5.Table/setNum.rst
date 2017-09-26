.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

setNum()
========

เก็บค่า Float ไว้ในแถวและคอลัมน์ที่กำหนดไว้ของ Table แถวถูกระบุโดย ID ของมันในขณะที่คอลัมน์อาจถูกระบุโดย ID หรือชื่อของ

.. Stores a Float value in the Table's specified row and column.
.. The row is specified by its ID, while the column may be specified
.. by either its ID or title.

**รูปแบบการใช้งาน**

setNum ( row, column, value )

**พารามิเตอร์**

- ``row``  Number: ID แถว

- ``column``  String,Number: คอลัมน์ ID (จำนวน) หรือชื่อ (สตริง)

- ``value``  Number: ค่าที่จะกำหนด

.. ``row``  Number: row ID
.. ``column``  String,Number: column ID (Number) or title (String)
.. ``value``  Number: value to assign

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
	  table.setNum(1, "id", 1);
	
	  print(table.getColumn(0));
	  //["0", 1, "2"]
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

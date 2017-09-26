.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

getNum()
========

ดึงข้อมูล Float จากแถวและคอลัมน์ที่กำหนดไว้ของ Table แถวถูกระบุโดย ID ของมันในขณะที่คอลัมน์อาจถูกระบุโดย ID หรือชื่อของ

.. Retrieves a Float value from the Table's specified row and column.
.. The row is specified by its ID, while the column may be specified by
.. either its ID or title.

**รูปแบบการใช้งาน**

getNum ( row, column )

**พารามิเตอร์**

- ``row``  Number: ID แถว

- ``column``  String,Number: columnName (string) หรือ ID (number)

.. ``row``  Number: row ID
.. ``column``  String,Number: columnName (string) or ID (number)

**ค่าที่ส่งออกมา**

- Number: 

.. Number: 

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
	  print(table.getNum(1, 0) + 100);
	  //id 1 + 100 = 101
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

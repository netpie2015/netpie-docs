.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

findRow()
=========

ค้นหาแถวแรกในตารางที่มีค่าที่ให้ไว้และส่งกลับการอ้างอิงไปยังแถวนั้น แม้ว่าจะมีแถวหลายแถวที่เป็นไปได้การจับคู่จะมีการส่งคืนเฉพาะแถวที่ตรงกันเท่านั้น คอลัมน์เพื่อค้นหาอาจระบุโดย ID หรือชื่อ

.. Finds the first row in the Table that contains the value
..  provided, and returns a reference to that row. Even if
..  multiple rows are possible matches, only the first matching
..  row is returned. The column to search may be specified by
..  either its ID or title.

**รูปแบบการใช้งาน**

findRow ( value, column )

**พารามิเตอร์**

- ``value``  String: ค่าที่จับคู่

- ``column``  Number,String: หมายเลขประจำตัวหรือชื่อของคอลัมน์ที่ต้องการค้นหา

.. ``value``  String: The value to match
.. ``column``  Number,String: ID number or title of the column to search

**ค่าที่ส่งออกมา**

- p5.TableRow: 

.. p5.TableRow: 

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
	  //find the animal named zebra
	  var row = table.findRow("Zebra", "name");
	  //find the corresponding species
	  print(row.getString("species"));
	}

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.

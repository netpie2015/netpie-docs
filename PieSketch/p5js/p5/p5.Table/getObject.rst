.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

getObject()
===========

เรียกข้อมูลตารางทั้งหมดและส่งคืนเป็นวัตถุ ถ้าชื่อคอลัมน์ถูกส่งผ่านไปวัตถุแต่ละแถวจะถูกเก็บไว้พร้อมกับแอตทริบิวต์นั้นเป็นชื่อของมัน

.. Retrieves all table data and returns as an object. If a column name is
.. passed in, each row object will be stored with that attribute as its
.. title.

**รูปแบบการใช้งาน**

getObject ( headerColumn )

**พารามิเตอร์**

- ``headerColumn``  String: ชื่อของคอลัมน์ที่ควรใช้เพื่อตั้งชื่อเรื่องแต่ละแถว (ไม่จำเป็น)

.. ``headerColumn``  String: Name of the column which should be used to title each row object (optional)

**ค่าที่ส่งออกมา**

- Object: 

.. Object: 

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
	  var tableObject = table.getObject();
	
	  print(tableObject);
	  //outputs an object
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

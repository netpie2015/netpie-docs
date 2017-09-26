.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

addColumn()
===========

ใช้ addColumn () เพื่อเพิ่มคอลัมน์ใหม่ลงในอ็อบเจ็กต์ Table โดยปกติคุณจะต้องระบุชื่อเพื่อให้คอลัมน์สามารถอ้างอิงได้ง่ายในภายหลังโดยใช้ชื่อ (หากไม่มีชื่อระบุชื่อคอลัมน์ใหม่จะเป็น null)

.. Use addColumn() to add a new column to a Table object.
..  Typically, you will want to specify a title, so the column
..  may be easily referenced later by name. (If no title is
..  specified, the new column's title will be null.)

**รูปแบบการใช้งาน**

addColumn ( [title] )

**พารามิเตอร์**

- ``title``  String: ชื่อของคอลัมน์ที่ระบุ

.. ``title``  String: title of the given column

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
	  table.addColumn("carnivore");
	  table.set(0, "carnivore", "no");
	  table.set(1, "carnivore", "yes");
	  table.set(2, "carnivore", "no");
	
	  //print the results
	  for (var r = 0; r < table.getRowCount(); r++)
	    for (var c = 0; c < table.getColumnCount(); c++)
	      print(table.getString(r, c));
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

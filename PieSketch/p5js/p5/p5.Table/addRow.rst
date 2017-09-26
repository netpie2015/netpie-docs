.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

addRow()
========

ใช้ addRow () เพื่อเพิ่มแถวข้อมูลใหม่ลงในอ็อบเจ็กต์ p5.Table โดยค่าเริ่มต้นจะสร้างแถวว่างไว้ โดยปกติคุณจะเก็บข้อมูลอ้างอิงไปยังแถวใหม่ในอ็อบเจ็กต์ TableRow (ดู newRow ในตัวอย่างข้างต้น) จากนั้นตั้งค่าแต่ละค่าโดยใช้ set () ถ้ามีการรวมอ็อบเจ็กต์ p5.TableRow เป็นพารามิเตอร์แถวนั้นจะถูกทำซ้ำและเพิ่มลงในตาราง

.. Use addRow() to add a new row of data to a p5.Table object. By default,
..  an empty row is created. Typically, you would store a reference to
..  the new row in a TableRow object (see newRow in the example above),
..  and then set individual values using set().
..  If a p5.TableRow object is included as a parameter, then that row is
..  duplicated and added to the table.
**รูปแบบการใช้งาน**

addRow ( [row] )

**พารามิเตอร์**

- ``row``  p5.TableRow: แถวที่จะเพิ่มลงในตาราง

.. ``row``  p5.TableRow: row to be added to the table

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
	  //add a row
	  var newRow = table.addRow();
	  newRow.setString("id", table.getRowCount() - 1);
	  newRow.setString("species", "Canis Lupus");
	  newRow.setString("name", "Wolf");
	
	  //print the results
	  for (var r = 0; r < table.getRowCount(); r++)
	    for (var c = 0; c < table.getColumnCount(); c++)
	      print(table.getString(r, c));
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

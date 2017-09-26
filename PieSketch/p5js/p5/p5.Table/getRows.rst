.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

getRows()
=========

เรียกแถวทั้งหมดจากตาราง ส่งกลับอาร์เรย์ของ p5.TableRows

.. Gets all rows from the table. Returns an array of p5.TableRows.

**รูปแบบการใช้งาน**

getRows ( )

**ค่าที่ส่งออกมา**

- Array.<p5.TableRow>: อาร์เรย์ของ p5.TableRows

.. Array.<p5.TableRow>: Array of p5.TableRows

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
	  var rows = table.getRows();
	
	  //warning: rows is an array of objects
	  for (var r = 0; r < rows.length; r++)
	    rows[r].set("name", "Unicorn");
	
	  //print the results
	  for (var r = 0; r < table.getRowCount(); r++)
	    for (var c = 0; c < table.getColumnCount(); c++)
	      print(table.getString(r, c));
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.

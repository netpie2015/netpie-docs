.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

matchRows()
===========

Finds the rows in the Table that match the regular expression provided,
 and returns references to those rows. Returns an array, so for must be
 used to iterate through all the rows, as shown in the example. The
 column to search may be specified by either its ID or title.

**รูปแบบการใช้งาน**

matchRows ( regexp, [column] )

**พารามิเตอร์**

- ``regexp``  String: The regular expression to match

- ``column``  String,Number: The column ID (number) or title (string)


**ค่าที่ส่งออกมา**

- Array.<p5.TableRow>: An Array of TableRow objects


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var table;
	
	 function setup() {
	
	   table = new p5.Table();
	
	   table.addColumn('name');
	   table.addColumn('type');
	
	   var newRow = table.addRow();
	   newRow.setString('name', 'Lion');
	   newRow.setString('type', 'Mammal');
	
	   newRow = table.addRow();
	   newRow.setString('name', 'Snake');
	   newRow.setString('type', 'Reptile');
	
	   newRow = table.addRow();
	   newRow.setString('name', 'Mosquito');
	   newRow.setString('type', 'Insect');
	
	   newRow = table.addRow();
	   newRow.setString('name', 'Lizard');
	   newRow.setString('type', 'Reptile');
	
	   var rows = table.matchRows('R.*', 'type');
	   for (var i = 0; i < rows.length; i++) {
	     print(rows[i].getString('name') + ': ' + rows[i].getString('type'));
	   }
	 }
	 // Sketch prints:
	 // Snake: Reptile
	 // Lizard: Reptile

	</script>

	<br><br>

.. toctree::


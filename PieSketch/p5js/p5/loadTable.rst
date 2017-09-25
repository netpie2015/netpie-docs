.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

loadTable()
===========

Reads the contents of a file or URL and creates a p5.Table object with
its values. If a file is specified, it must be located in the sketch's
"data" folder. The filename parameter can also be a URL to a file found
online. By default, the file is assumed to be comma-separated (in CSV
format). Table only looks for a header row if the 'header' option is
included.
Possible options include:

csv - parse the table as comma-separated values
tsv - parse the table as tab-separated values
header - this table has a header (title) row


When passing in multiple options, pass them in as separate parameters,
seperated by commas. For example:


  loadTable("my_csv_file.csv", "csv", "header")


 All files loaded and saved use UTF-8 encoding.
This method is asynchronous, meaning it may not finish before the next
line in your sketch is executed. Calling loadTable() inside preload()
guarantees to complete the operation before setup() and draw() are called.
Outside of preload(), you may supply a callback function to handle the
object:


**รูปแบบการใช้งาน**

loadTable ( filename, [options], [callback], [errorCallback] )

**พารามิเตอร์**

- ``filename``  String: name of the file or URL to load

- ``options``  String: "header" "csv" "tsv"

- ``callback``  function: function to be executed after loadTable() completes. On success, the Table object is passed in as the first argument.

- ``errorCallback``  function: function to be executed if there is an error, response is passed in as first argument


**ค่าที่ส่งออกมา**

- Object: Table object containing data


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	// Given the following CSV file called "mammals.csv"
	// located in the project's "assets" folder:
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
	  //the file can be remote
	  //table = loadTable("http://p5js.org/reference/assets/mammals.csv",
	  //                  "csv", "header");
	}
	
	function setup() {
	  //count the columns
	  print(table.getRowCount() + " total rows in table");
	  print(table.getColumnCount() + " total columns in table");
	
	  print(table.getColumn("name"));
	  //["Goat", "Leopard", "Zebra"]
	
	  //cycle through the table
	  for (var r = 0; r < table.getRowCount(); r++)
	    for (var c = 0; c < table.getColumnCount(); c++) {
	      print(table.getString(r, c));
	    }
	}

	</script>

	<br><br>

.. toctree::


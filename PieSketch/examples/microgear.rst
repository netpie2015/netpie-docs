.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

การสื่อสารระหว่าง p5.js ผ่าน NETPIE
========================================

เป็นการประยุกต์การใช้งานร่วมกันระหว่าง p5.js กับ Microgear library ทำให้สามารถที่จะสื่อสารถึงกันได้ทุกที่ผ่าน NETPIE platform ตัวอย่างเช่น การสื่อสารพูดคุยกันระหว่าง Area1 กับ Area2 

Area 1

.. raw:: html

	<script type="text/p5" data-height="400" data-preview-width="400">
	var microgear, text;
	var TOPICID = "TOPIC_ID";

	var APPID = "demop5js";
	var KEY = "I49roGVvec8byUS";
	var SECRET = "nbSEmYXZxH60HJQILCQPmqYLD";

	var ALIAS1 = "area1"+TOPICID;
	var TOPIC1 = "/"+TOPICID+"/"+ALIAS1;

	var ALIAS2 = "area2"+TOPICID;
	var TOPIC2 = "/"+TOPICID+"/"+ALIAS2;

	var xpos = 0;
	var ypos = 0;
	var xspeed = 2;
	var yspeed = 2;
	var count = 0;
	var sync = false;
	var isOnline = false;

	function sendMsg(){
        if(count == 1) microgear.publish(TOPIC2,xpos+","+ypos);
        count++;
	}

	function onPresent(event) {
		if((event.type == "online" || event.type == "aliased") && event.alias == ALIAS2) sync = true;
		else if(event.type == "offline" && event.alias == ALIAS2) sync = false;
	}

	function onMessage(topic, msg) {
        count = 0;
        var m = msg.split(",");
        xpos = parseInt(m[0]);
        ypos = 320;
  		yspeed = -2;
    }

	function onConnected() {
        microgear.setAlias(ALIAS1);
        microgear.subscribe(TOPIC1);
    	isOnline = true;
        text.html("Now I am connected with netpie...");
	}


	function setup()
	{
        createCanvas(400, 320);
        text = createSpan("_____");
        text.position(10,50);

        microgear = Microgear.create({key:KEY, secret:SECRET, alias:ALIAS1});
        microgear.on('connected',onConnected);
        microgear.on('message',onMessage);
        microgear.on('present',onPresent);
        microgear.connect(APPID);
	}

	function draw()
	{
		background(255);
		fill(255, 0, 0);
		stroke(0);
		ellipseMode(CENTER);

		xpos = xpos + xspeed;
		ypos = ypos + yspeed;

		if((xpos > width) || (xpos < 0)) {
			xspeed = xspeed * -1;
		}

		if(ypos < 0) {
			yspeed = 2;
		}

		if(!sync) {
			if(ypos > height) {
				yspeed = yspeed * -1;
			}
			ellipse(xpos, ypos, 25, 25);
			fill(0);
		} else {
			if(ypos > height && count == 0 && isOnline) {
				count = 1;
				sendMsg();
			}

			if(ypos <= height) {
				ellipse(xpos, ypos, 25, 25);
				fill(0);
			}
		}
	}
	</script>
	<p></p>

Area 2

.. raw:: html

	<script type="text/p5" data-height="400" data-preview-width="400">
	var microgear, text;
	var TOPICID = "TOPIC_ID";

	var APPID = "demop5js";
	var KEY = "I49roGVvec8byUS";
	var SECRET = "nbSEmYXZxH60HJQILCQPmqYLD";

	var ALIAS1 = "area1"+TOPICID;
	var TOPIC1 = "/"+TOPICID+"/"+ALIAS1;

	var ALIAS2 = "area2"+TOPICID;
	var TOPIC2 = "/"+TOPICID+"/"+ALIAS2;

	var xpos = 0;
	var ypos = 0;
	var xspeed = 2;
	var yspeed = 2;
	var count = 0;
	var sync = false;
	var isOnline = false;
	var isStarted = false;

	function sendMsg(){
        if(count == 1) microgear.publish(TOPIC1,xpos+","+ypos);
        count++;
	}

	function onPresent(event) {
	    if((event.type == "online" || event.type == "aliased") && event.alias == ALIAS1) sync = true;
	    else if(event.type == "offline" && event.alias == ALIAS1) sync = false;
	}

	function onMessage(topic, msg) {
        count = 0;
        isStarted = true;
        var m = msg.split(",");
        xpos = parseInt(m[0]);
        ypos = 0;
  		yspeed = 2;
	}

	function onConnected() {
        microgear.setAlias(ALIAS2);
        microgear.subscribe(TOPIC2);
	    isOnline = true;
        text.html("Now I am connected with netpie...");
	}


	function setup() {
        createCanvas(400, 320);
        text = createSpan("_____");
        text.position(10,50);

        microgear = Microgear.create({key:KEY, secret:SECRET, alias:ALIAS1});
        microgear.on('connected',onConnected);
        microgear.on('message',onMessage);
        microgear.on('present',onPresent);
        microgear.connect(APPID);
	}

	function draw()
	{
		if(isStarted) {
		    background(255);
		    fill(255, 0, 0);
		    stroke(0);
		    ellipseMode(CENTER);

		    xpos = xpos + xspeed;
		    ypos = ypos + yspeed;

		    if((xpos > width) || (xpos < 0)) {
	            xspeed = xspeed * -1;
		    }

		    if(ypos > height) {
		    	yspeed = -2;
		    }

		    if(!sync) {
	            if(ypos < 0) {
                    yspeed = yspeed * -1;
	            }
	            ellipse(xpos, ypos, 25, 25);
	            fill(0);
		    } else {
	            if(ypos < 0 && count == 0 && isOnline) {
                    count = 1;
                    sendMsg();
	            }

	            if(ypos >= 0) {
                    ellipse(xpos, ypos, 25, 25);
                    fill(0);
	            }
		    }
		}
	}
	</script>
	<p></p>

	<script>
		var text = "";
		var possible = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789";

		for (var i = 0; i < 10; i++)
			text += possible.charAt(Math.floor(Math.random() * possible.length));

		for(var i=0; i<document.getElementsByTagName('script').length; i++){
			//console.log(document.getElementsByTagName('script')[i].outerHTML);
			document.getElementsByTagName('script')[i].outerHTML = document.getElementsByTagName('script')[i].outerHTML.replace("TOPIC_ID",text);
		}
	</script>

.. toctree::
	:hidden:

	การวาดภาพกราฟฟิก <examples/graphic>
	การควบคุมเปลี่ยนแปลงสี <examples/control_rgb>
	ภาพเคลี่อนไหว 2D <examples/2d>
	ภาพเคลี่อนไหว 3D <examples/3d>
	การสื่อสารระหว่าง p5.js ผ่าน NETPIE <examples/microgear>


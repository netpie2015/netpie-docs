.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

ortho()
=======

Setup ortho camera

**รูปแบบการใช้งาน**

ortho ( left, right, bottom, top, near, far )

**พารามิเตอร์**

- ``left``  Number: camera frustum left plane

- ``right``  Number: camera frustum right plane

- ``bottom``  Number: camera frustum bottom plane

- ``top``  Number: camera frustum top plane

- ``near``  Number: camera frustum near plane

- ``far``  Number: camera frustum far plane


**ค่าที่ส่งออกมา**

- p5: the p5 object


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	//drag mouse to toggle the world!
	//there's no vanish point
	function setup(){
	  createCanvas(100, 100, WEBGL);
	  ortho(-width/2, width/2, height/2, -height/2, 0, 500);
	}
	function draw(){
	 background(200);
	 orbitControl();
	 for(var i = -1; i < 2; i++){
	    for(var j = -2; j < 3; j++){
	      push();
	      translate(i*160, 0, j*160);
	      box(40, 40, 40);
	      pop();
	    }
	  }
	}


	</script>

	<br><br>

.. toctree::


ghosts-and-supernaturals
========================
<!doctype html>
<html>
	<head>
		<meta charset = "utf-8" />
		<title>PH's Supernaturals</title>
		<link href='http://fonts.googleapis.com/css?family=Source+Sans+Pro:200,300,400,600' rel='stylesheet' type='text/css'>
		<link href="temp.css" rel="stylesheet" type="text/css" media="screen" />
		<link href="styles.css" rel="stylesheet" type="text/css" media="screen" />
		<script src="slideshow-home.js"></script>
		<script src="witch.js"></script>
	
		<script type="text/javascript">
			function play(){
				var sound = new Audio ("kapre evil laugh.mp3");
				sound.play();
			}
			 function stop(){
				var sound = new Audio ("kapre evil laugh.mp3");
				sound.stop();
			}
			
			function playB(){
				var sound1 = new Audio ("wakwak.mp3");
				sound1.play();
			}
			function stop1(){
				var sound1 = new Audio ("wakwak.mp3");
				sound1.stop();
			}
			
			function playC(){
				var sound2 = new Audio ("Any3.mp3");
				sound2.play();
			}
			function stop2(){
				var sound2 = new Audio ("Any3.mp3");
				sound2.stop();
			 }	
			function playD(){
				var sound3 = new Audio ("any5.mp3");
				sound3.play();
			}
			function stop3(){
				var sound3 = new Audio ("any5.mp3");
				sound3.stop();
			 }	 
			 function playE(){
				var sound4 = new Audio ("Witch laugh2.mp3");
				sound4.play();
			}
			function stop4(){
				var sound4 = new Audio ("Witch laugh2.mp3");
				sound4.stop();
			 }
			 function playF(){
				var sound5 = new Audio ("any4.mp3");
				sound5.play();
			}
			function stop5(){
				var sound5 = new Audio ("any4.mp3");
				sound5.stop();
			 }
	 		function playG(){
				var sound6 = new Audio ("ANY.mp3");
				sound6.play();
			}
			function stop6(){
				var sound6 = new Audio ("ANY.mp3");
				sound6.stop();
			 }
			function playH(){
				var sound7 = new Audio ("mambabarang.mp3");
				sound7.play();
			}
			function stop7(){
				var sound7 = new Audio ("mambabarang.mp3");
				sound7.stop();
			 }
			function playI(){
				var sound8 = new Audio ("manananggal.mp3");
				sound8.play();
			}
			function stop8(){
				var sound8 = new Audio ("manananggal.mp3");
				sound8.stop();
			 }
			 function playJ(){
				var sound9 = new Audio ("Any3.mp3");
				sound9.play();
			}
			function stop9(){
				var sound9 = new Audio ("Any3.mp3");
				sound9.stop();
			 }
			function playK(){
				var sound10 = new Audio ("tikbalang.mp3");
				sound10.play();
			}
			function stop10(){
				var sound10 = new Audio ("tikbalang.mp3");
				sound10.stop();
			 }
			function playL(){
				var sound11 = new Audio ("tiyanak.mp3");
				sound11.play();
			}
			function stop11(){
				var sound11 = new Audio ("tiyanak.mp3");
				sound11.stop();
			 }

		</script>
	</head>

	<body>
	<script type="text/javascript">
		play();
		setTimeout("stop()",10000);
		setTimeout("playB()",10000);
		
		setTimeout("stop1()",10000);
		setTimeout("playC()",10000);
		
		setTimeout("stop2()",10000);	
		setTimeout("playD()",10000);
		
		setTimeout("stop3()",10000);	
		setTimeout("playE()",10000);
		
		setTimeout("stop4()",10000);	
		setTimeout("playF()",10000);
		
		
		setTimeout("stop5()",10000);	
		setTimeout("playG()",10000);
		
		setTimeout("stop6()",10000);	
		setTimeout("playH()",10000);
		
		setTimeout("stop7()",10000);	
		setTimeout("playI()",10000);
		

		setTimeout("stop8()",10000);
		setTimeout("playJ()",10000);
		
		setTimeout("stop9()",10000);	
		setTimeout("playK()",10000);
		
		setTimeout("stop10()",10000);
		setTimeout("playL()",10000);
		
		setTimeout("stop11()",10000);
		
	</script>

	<div id="wrapper">
		<div class='witch' id='witch1'></div>
			<div id="header-wrapper">
				<div id="header">
					<div id="logo">
						<img style="margin-left:-300px;"src="logo5.png" height="300" width="1550">
						
					</div>
				</div>
			</div>
			<div id="menu">
				<ul>
					<li><a href="home-s.html" style="background: #FFFFFF; color: #F44C31;">MYTHICAL CREATURES</a>
					</li>
					<li><a href="ghost.html">GHOSTS</a></li>
					<li><a href="ladies.html">HORROR LADIES</a></li>
					<li><a href="memory.html">GAMES</a></li>
					<li><a href="horrorstories.html">STORIES</a></li>
					<li><a href="aboutus.html">ABOUT US</a></li>
				</ul>
			</div>
			<!-- end #menu -->
			<div id="page">
				<div class="h1" style="text-align:center; color:red;"><h1>Mythical Creatures in the Philippines</h1>
				</div>
				<hr size="2" width="50%"></hr>
				<a href="mList.html" style="text-align:center; color:red;"><p>See the List</p></a>
				<div id="page-bgtop">
					<div id="page-bgbtm">
						<div id="content">
								<div class="entry">								
								<script type="text/javascript">
									witchImg = document.getElementById("witch1");
									//document.write("<div class='witch' id='witch1'></div>");
									witchImg.style.backgroundImage = "url('"+witch1.imageLink+"')";
									
									moveWitch();
									
									function moveWitch(){
										var randY = Math.floor(Math.random()*1);
										var randX = Math.floor(Math.random()*1);
										
										switch(witch1.facing){
											case FACE_DIR.LEFT:
												if(randX > witch1.position.x){
													console.log("from " + witch1.position.x + " to " + randX);
													console.log("switch to right");
													witch1.facing = FACE_DIR.RIGHT;
													witchImg.style.transform = "rotate-left(360deg)";
												}
												break;
											case FACE_DIR.RIGHT:
												if(randX < witch1.position.x){
													console.log("to " + witch1.position.x + " from " + randX);
													console.log("switch to left");
													witch1.facing = FACE_DIR.LEFT;
													witchImg.style.transform = "rotate(360deg)";
												}
												break;
											}

										witch1.position.x = randX;
										witch1.position.y = randY;

										witchImg.style.marginTop = (randY) + "%";
										witchImg.style.marginRight = (64 - randX) + "%";
										setTimeout("moveWitch()",1000);
									}
								</script>
									<table style="margin-left:250px;border:10px solid #891100;background-color:#891100;" align="center"> 
										<tr> 
											<td>
												<img name="slide" id="slide" alt ="Mythical Creatures" height="550" width="1100" src="MC/c1.jpg" style="color:white;padding:10px;"/> 
											</td> 
										</tr> 

										<tr>
											<td align="center"style="font:25px arial; color:white;"> 
												<div id ="mydiv"></div>
											</td> 
										</tr> 
									</table> 
								</div>
							<div style="clear: both;">&nbsp;</div>
						</div>
						<div style="clear: both;">&nbsp;</div>
					</div>
				</div>
			</div>
		</div>
		<div id="footer">
		<hr size="2" width="100%"></hr>
			<p>Copyright (c) 2014 supernaturals.com | All rights reserved. | Design by JS Group</a>.</p>
		</div>
	</body>
</html>	

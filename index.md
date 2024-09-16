---
layout: base
title: Arya's Website
description: Welcome.
hide: true
---
<h1>👋 Welcome to my Website...</h1>
<br>
<link href="https://fonts.googleapis.com/css?family=Press+Start+2P" rel="stylesheet">
<div class="sky">
	<div class="scorebar">
		<style>
			.topline-mario{position:absolute;}
			.topline-world{position:absolute; left:55%;}
			.topline-time{position:absolute; left: 85%;}
			{position:absolute; top: 90px;}
			.bottomline-coin{position:absolute; top: 80px; left:30%;}
			.bottomline-world{position:absolute; top: 90px; left:55.7%;}
			.bottomline-time{position:absolute; top: 90px; left:85.5%;}
		</style>
		
			
</div>
<div class="ground">
	<div class="skyblocks">
		<img class="brick" src="https://raw.githubusercontent.com/LantareCode/random-this-and-thats/master/CSS/SuperMario-Animation/images/Bricks.gif" height="70px;">
		<img class="brick" src="https://raw.githubusercontent.com/LantareCode/random-this-and-thats/master/CSS/SuperMario-Animation/images/QuestionBlock.gif" height="70px;">
		<img class="brick" src="https://raw.githubusercontent.com/LantareCode/random-this-and-thats/master/CSS/SuperMario-Animation/images/Bricks.gif" height="70px;">
		<img class="brick" src="https://raw.githubusercontent.com/LantareCode/random-this-and-thats/master/CSS/SuperMario-Animation/images/Bricks.gif" height="70px;">
	</div>


</div>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Moving Image</title>
    <style>
        /* Container to hold the image */
        .container {
            width: 100vw;
            height: 18vh;
            overflow: hidden;
            position: relative;
        }

        /* Image styling */
        .moving-img {
            width: 125px;
            position: absolute;
            top: 50%; /* Center vertically */
            left: -100px; /* Start off screen */
            transform: translateY(-50%);
            animation: moveAcross 5s linear infinite;
        }

        /* Animation */
        @keyframes moveAcross {
            0% {
                left: -100px; /* Start off screen on the left */
            }
            100% {
                left: 100vw; /* Move to the right side of the screen */
            }
        }
    </style>
</head>
    <div class="container">
        <img src="{{site.baseurl}}/images/mario.gif" alt="Moving Image" class="moving-img">
    </div>
</html>



<table>
    <tr>
        <td width = "150"><img src="{{site.baseurl}}/images/india.png" height="70" title="Pair" alt=""></td>
        <td><a href="index_submenu.html">Valorant Blog(MiniProject)</a></td>
        <td><a href="{{site.baseurl}}/pair/habits">Future Submenu 2</a></td>
        <td><a href="{{site.baseurl}}/pair/habits">Future Submenu 3</a></td>
    </tr>
</table>


<!--tag>
<main>
  <h1>The Most Popular Computer Languages:</h1>
  <a href="https://www.coursera.org/articles/popular-programming-languages">Source</a>
  

  <article>
    <h3>1. JavaScipt</h3>
   
  </article>

  <article>
    <h3>2. HTML/CSS</h3>
    
  </article>

  <article>
    <h3>3. Python</h3>
   
  </article>
</main>
-->
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
            .topline-mario { position: absolute; }
            .topline-world { position: absolute; left: 55%; }
            .topline-time { position: absolute; left: 85%; }
            { position: absolute; top: 90px; }
            .bottomline-coin { position: absolute; top: 80px; left: 30%; }
            .bottomline-world { position: absolute; top: 90px; left: 55.7%; }
            .bottomline-time { position: absolute; top: 90px; left: 85.5%; }
        </style>
    </div>
    
    <!-- Skyblocks preserved -->
    <div class="ground">
        <div class="skyblocks">
            <img class="brick" src="https://raw.githubusercontent.com/LantareCode/random-this-and-thats/master/CSS/SuperMario-Animation/images/Bricks.gif" height="70px;">
            <img class="brick" src="https://raw.githubusercontent.com/LantareCode/random-this-and-thats/master/CSS/SuperMario-Animation/images/QuestionBlock.gif" height="70px;">
            <img class="brick" src="https://raw.githubusercontent.com/LantareCode/random-this-and-thats/master/CSS/SuperMario-Animation/images/Bricks.gif" height="70px;">
            <img class="brick" src="https://raw.githubusercontent.com/LantareCode/random-this-and-thats/master/CSS/SuperMario-Animation/images/Bricks.gif" height="70px;">
        </div>
    </div>
</div>

<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Moving Mario</title>
    <style>
        /* Container to hold the image */
        .container {
            width: 50vw;
            height: 25vh;
            overflow: hidden;
            position: relative;

        }

        /* Mario image styling */
        .moving-img {
            width: 175px;
            position: absolute;
            top: 0; /* Start at the top left */
            left: 0; /* Start at the top left */
        }
    </style>
</head>
<body>
    <div class="container">
        <img src="{{site.baseurl}}/images/mario.gif" alt="Moving Mario" class="moving-img" id="mario">
    </div>

    <script>
        // Get the Mario element and container
        const mario = document.getElementById('mario');
        const container = document.querySelector('.container');

        // Initialize Mario's position relative to the container
        let xPos = 0; // Start at 0 (top-left corner)
        let yPos = 0; // Start at 0 (top-left corner)

        // Function to move Mario
        function moveMario(event) {
            switch (event.key) {
                case 'ArrowUp':
                    yPos -= 10; // Move up
                    break;
                case 'ArrowDown':
                    yPos += 10; // Move down
                    break;
                case 'ArrowLeft':
                    xPos -= 10; // Move left
                    break;
                case 'ArrowRight':
                    xPos += 10; // Move right
                    break;
            }

            // Prevent Mario from going off-screen within the container
            if (xPos < 0) xPos = 0;
            if (yPos < 0) yPos = 0;
            if (xPos > container.clientWidth - 125) xPos = container.clientWidth - 125; // 125 is Mario's width
            if (yPos > container.clientHeight - 125) yPos = container.clientHeight - 125; // 125 is Mario's height

            // Update Mario's position
            mario.style.left = xPos + 'px';
            mario.style.top = yPos + 'px';
        }

        // Listen for arrow key presses
        window.addEventListener('keydown', moveMario);
    </script>
</body>
</html>

<td>
  <a href="personalblog.html">
    <button style="background-color: #4CAF50; color: white; padding: 10px 20px; font-size: 16px; border: none; cursor: pointer;">
      Visit My Sprint 2 Blog
    </button>
  </a>
</td>



<table>
    <tr>
        <td width="150">
            <img src="{{site.baseurl}}/images/india.png" height="70" title="Pair" alt="" onclick="playAudio()">
        </td>
        <td><a href="index_submenu.html">Valorant Blog(MiniProject)</a></td>
        <td><a href="snake.html">Snake Game</a></td>
        <td><a href="cookieclicker.html">Cookie Clicker</a></td>
        <td><a href="calculator.html">Calculator</a></td>
        <td><a href= "http://127.0.0.1:4100/arya/itunes/">Itunes</a></td>

        
    </tr>
</table>


<audio id="flagSound" src="{{site.baseurl}}/images/india.mp3"></audio>

<script>
    function playAudio() {
        const audio = document.getElementById('flagSound');
        audio.currentTime = 0;  // Reset audio to the start
        audio.play();           // Play the sound
    }
</script>





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
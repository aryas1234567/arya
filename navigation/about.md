---
layout: page
title: About Me
permalink: /about/
---
Hi, my name is Arya Savlani and I am a sophomore at Del Norte. I enjoy playing sports, hanging out with my friends, and watching movies. I have 2 loving parents and an older sister.
<br>

Learn more about me...

<button onclick="showRandomFact()">Click Here</button>

<p id="fact"></p>

<script>
  const MeFacts = [
    "My favorite color is dark purple.",
    "I love Mexican food, especially street tacos.",
    "I think pineapples are good on pizza.",
    "My favorite video game at the moment is Minecraft.",
    "My parents are both in computer science fields.",
    "I love watching movies, my favorite movie is Django Unchained, watch it!"
  ];

  // Show random fact
  function showRandomFact() {
    const randomIndex = Math.floor(Math.random() * MeFacts.length);
    const randomFact = MeFacts[randomIndex];
    document.getElementById('fact').textContent = randomFact;
  }
</script>

<h3>Things I love:</h3>

<ul>
  <li><img src="{{site.baseurl}}/images/tenn.jpg" alt="Tennis" width="300" height="300"><p style ="font-size:16px;display:inline-block">&nbsp; Playing Tennis</p></li>
</ul>
<br>
<ul>
  <li><img src="{{site.baseurl}}/images/soccer.jpg" alt="Soccer" width="450" height="300"><p style ="font-size:16px;display:inline-block;"> &nbsp; Playing Soccer</p></li>
</ul>
<br>
<ul>
  <li><img src="{{site.baseurl}}/images/setup.jpg" alt="Tennis" width="300" height="300"><p style ="font-size:16px;display:inline-block">&nbsp;  Playing Video Games</p></li>
</ul>



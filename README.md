walkabout
=========

<p>"Hello World" for a virtual world using Three.js</p>

<p>This mashup is a heavily modified tps from Yomotsu's example linked at the Threejs.org wiki.
In it, you 'll find javascript using Three.js to create:

<ul>
<li>Skybox</li>
<li>Heightmap terrain</li>
<li>Very simple water mesh</li>
<li>Character walk on uneven terrain using a Raycaster</li>
<li>Multiplayer through a node.js Websocket server</li>
</ul>

Each of the components was created using code from others' examples, the sources are cited in
the source code.</p>

<p>You can simply load index.html in your browser and walk about the island by yourself, but the real
fun is in putting it on an accessible web server and running server.js with the appropriate URLs
inserted in both index.html and server.js.  There is a variable in index.html called multiplayer
that is currently set to true, but you should change that to false if you're just going to walk
about the island without the company of others.</p>

<p>Of Note:
<ul>
<li>Heightmap terrain handling is currently hard-coded for 128x128 grayscale images</li>
<li>Google Chrome runs the world a lot faster than Firefox, but mousewheel zoom doesn't work right yet.</li>
<li>There's an undocumented command, the "t" key, which will transport you instantaneously to the 
highest point on the terrain.</li>
<li>On steep terrain,  you'll notice that your character's feet are occasionally below the terrain 
surface.  It's 'hello world', not Second Life, so learn to love it, or send me a patch to improve
it. :)</li>
<li>Running the server.js requires node.js, as well as the websocket library (npm install ws)</li>
</ul>


<p>While I intend to make minor changes, I'm not going to engage in an extensive issues/bug tracking
campaign to turn it into a full-featured application.  Rather, I encourage folks to fork the project 
and do their own world, or just copy/paste and have fun with it.</p>

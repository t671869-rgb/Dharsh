CREATE TABLE contacts (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(100),
    email VARCHAR(100),
    message TEXT
);<!DOCTYPE html>
<html>
<head>
<title>Portfolio</title>
</head>
<body>
<h1>Dharshini T</h1>
<h2>B.Tech Information Technology</h2>

<h3>About Me</h3>
<p>I am a final year B.Tech IT student interested in Web Development and Cyber Security.</p>

<h3>Skills</h3>
<ul>
<li>HTML</li>
<li>CSS</li>
<li>JavaScript</li>
<li>Python</li>
<li>Java</li>
</ul>

<h3>Projects</h3>
<p>Online Portfolio Website</p>

<h3>Contact</h3>
<form>
<input type="text" placeholder="Name"><br><br>
<input type="email" placeholder="Email"><br><br>
<textarea placeholder="Message"></textarea><br><br>
<button type="submit">Submit</button>
</form>

</body>
</html>

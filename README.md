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
<!DOCTYPE html>
<html>
<head>
    <title>Task Management Application</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            margin-top: 50px;
        }

        input {
            padding: 10px;
            width: 250px;
        }

        button {
            padding: 10px;
            margin-left: 5px;
        }

        li {
            margin: 10px;
        }
    </style>
</head>
<body>

    <h2>Task Management Application</h2>

    <input type="text" id="taskInput" placeholder="Enter Task">
    <button onclick="addTask()">Add Task</button>

    <ul id="taskList"></ul>

    <script>
        function addTask() {
            let task = document.getElementById("taskInput").value;

            if(task === "") {
                alert("Enter a task!");
                return;
            }

            let li = document.createElement("li");
            li.innerHTML = task +
                " <button onclick='editTask(this)'>Edit</button>" +
                " <button onclick='deleteTask(this)'>Delete</button>";

            document.getElementById("taskList").appendChild(li);
            document.getElementById("taskInput").value = "";
        }

        function deleteTask(button) {
            button.parentElement.remove();
        }

        function editTask(button) {
            let newTask = prompt("Edit Task:", button.parentElement.firstChild.textContent);
            if(newTask != null) {
                button.parentElement.firstChild.textContent = newTask + " ";
            }
        }
    </script>

</body>
</html>

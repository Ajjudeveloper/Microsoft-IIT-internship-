# Microsoft-IIT-internship-TO DO LIST
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Advanced To-Do List</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #f4f4f4;
            transition: background 0.3s, color 0.3s;
        }
        .dark-mode {
            background-color: #121212;
            color: white;
        }
        .container {
            max-width: 400px;
            margin: 50px auto;
            padding: 20px;
            background: white;
            box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.2);
            border-radius: 10px;
        }
        .dark-mode .container {
            background: #1e1e1e;
            color: white;
        }
        button {
            background: #6200ea;
            color: white;
            padding: 10px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            margin-top: 10px;
        }
        button:hover {
            background: #3700b3;
        }
        input, select {
            padding: 8px;
            margin: 5px;
            width: calc(100% - 20px);
            border: 1px solid #ccc;
            border-radius: 5px;
        }
        ul {
            list-style: none;
            padding: 0;
        }
        li {
            background: #ddd;
            padding: 10px;
            margin: 5px 0;
            display: flex;
            justify-content: space-between;
            align-items: center;
            border-radius: 5px;
        }
        .dark-mode li {
            background: #444;
        }
        .clear-btn {
            background: red;
        }
    </style>
</head>
<body>

    <div class="container">
        <h2>To-Do List</h2>
        <button onclick="toggleDarkMode()">🌙 Dark Mode</button>

        <div class="input-area">
            <input type="text" id="taskInput" placeholder="Enter a task">
            <input type="date" id="deadline">
            <select id="priority">
                <option value="Low">Low Priority</option>
                <option value="Medium">Medium Priority</option>
                <option value="High">High Priority</option>
            </select>
            <button onclick="addTask()">Add Task</button>
        </div>

        <div class="filter-area">
            <input type="text" id="searchInput" placeholder="Search tasks..." onkeyup="searchTasks()">
            <select id="filterPriority" onchange="filterTasks()">
                <option value="All">All Priorities</option>
                <option value="High">High</option>
                <option value="Medium">Medium</option>
                <option value="Low">Low</option>
            </select>
            <button class="clear-btn" onclick="clearAllTasks()">Clear All</button>
        </div>

        <ul id="taskList"></ul>
    </div>

    <script>
        document.addEventListener("DOMContentLoaded", loadTasks);

        function addTask() {
            const taskInput = document.getElementById("taskInput");
            const deadline = document.getElementById("deadline").value;
            const priority = document.getElementById("priority").value;
            const taskText = taskInput.value.trim();

            if (taskText === "") {
                alert("Please enter a task!");
                return;
            }

            const task = { text: taskText, deadline, priority };
            let tasks = JSON.parse(localStorage.getItem("tasks")) || [];
            tasks.push(task);
            localStorage.setItem("tasks", JSON.stringify(tasks));

            taskInput.value = "";
            loadTasks();
        }

        function loadTasks() {
            const taskList = document.getElementById("taskList");
            taskList.innerHTML = "";

            let tasks = JSON.parse(localStorage.getItem("tasks")) || [];

            tasks.forEach((task, index) => {
                const li = document.createElement("li");
                li.innerHTML = `
                    ${task.text} - ${task.deadline} - <strong>${task.priority}</strong>
                    <button onclick="deleteTask(${index})">❌</button>
                `;
                taskList.appendChild(li);
            });
        }

        function deleteTask(index) {
            let tasks = JSON.parse(localStorage.getItem("tasks")) || [];
            tasks.splice(index, 1);
            localStorage.setItem("tasks", JSON.stringify(tasks));
            loadTasks();
        }

        function clearAllTasks() {
            if (confirm("Are you sure you want to clear all tasks?")) {
                localStorage.removeItem("tasks");
                loadTasks();
            }
        }

        function searchTasks() {
            const searchInput = document.getElementById("searchInput").value.toLowerCase();
            const tasks = document.querySelectorAll("#taskList li");

            tasks.forEach(task => {
                task.style.display = task.innerText.toLowerCase().includes(searchInput) ? "flex" : "none";
            });
        }

        function filterTasks() {
            const selectedPriority = document.getElementById("filterPriority").value;
            let tasks = JSON.parse(localStorage.getItem("tasks")) || [];
            
            const filteredTasks = selectedPriority === "All" ? tasks : tasks.filter(task => task.priority === selectedPriority);
            
            document.getElementById("taskList").innerHTML = "";
            filteredTasks.forEach((task, index) => {
                const li = document.createElement("li");
                li.innerHTML = `
                    ${task.text} - ${task.deadline} - <strong>${task.priority}</strong>
                    <button onclick="deleteTask(${index})">❌</button>
                `;
                document.getElementById("taskList").appendChild(li);
            });
        }

        function toggleDarkMode() {
            document.body.classList.toggle("dark-mode");
        }
    </script>

</body>
</html>

# EX_03-To-Do-List-using-JavaScript
## Date: 20.05.2025
```
NAME : Sri Harish B
REG NO : 212223220110
```
## AIM
To create a To-do Application with all features using JavaScript.

## ALGORITHM
### STEP 1
Build the HTML structure (index.html).

### STEP 2
Style the App (style.css).

### STEP 3
Plan the features the To-Do App should have.

### STEP 4
Create a To-do application using Javascript.

### STEP 5
Add functionalities.

### STEP 6
Test the App.

### STEP 7
Open the HTML file in a browser to check layout and functionality.

### STEP 8
Fix styling issues and refine content placement.

### STEP 9
Deploy the website.

### STEP 10
Upload to GitHub Pages for free hosting.

## PROGRAM
```<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>To-Do List</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #f0f0f0;
      text-align: center;
      margin-top: 50px;
    }

    .container {
      background: #fff;
      padding: 20px;
      width: 300px;
      margin: auto;
      border-radius: 10px;
      box-shadow: 0 0 10px gray;
    }

    input[type="text"] {
      padding: 10px;
      width: 70%;
      border: 1px solid #ccc;
      border-radius: 5px;
    }

    button {
      padding: 10px;
      margin-left: 5px;
      border: none;
      background-color: #28a745;
      color: white;
      border-radius: 5px;
      cursor: pointer;
    }

    ul {
      list-style-type: none;
      padding: 0;
      margin-top: 20px;
    }

    li {
      padding: 8px;
      border-bottom: 1px solid #ddd;
      display: flex;
      justify-content: space-between;
    }

    li button {
      background-color: red;
      color: white;
      border: none;
      padding: 5px;
      border-radius: 3px;
      cursor: pointer;
    }
  </style>
</head>
<body>
  <div class="container">
    <h2>To-Do List</h2>
    <input type="text" id="taskInput" placeholder="Add a new task">
    <button onclick="addTask()">Add</button>
    <ul id="taskList"></ul>
  </div>

  <script>
    function addTask() {
      const input = document.getElementById("taskInput");
      const taskText = input.value.trim();

      if (taskText === "") return;

      const li = document.createElement("li");
      li.textContent = taskText;

      const delBtn = document.createElement("button");
      delBtn.textContent = "Delete";
      delBtn.onclick = () => li.remove();

      li.appendChild(delBtn);
      document.getElementById("taskList").appendChild(li);

      input.value = "";
    }
  </script>
</body>
</html>
```

## OUTPUT
![image](https://github.com/user-attachments/assets/1da8f315-6ceb-4c74-bb42-11990e85d5ed)

## RESULT
The program for creating To-do list using JavaScript is executed successfully.

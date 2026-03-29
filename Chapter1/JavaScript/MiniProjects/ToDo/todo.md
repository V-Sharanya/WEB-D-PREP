🟢 Mini Project 1: Todo List (Core App)
🎯 Objective

Build a simple Todo app with:

📄 Base HTML
<input type="text" id="taskInput">
<button id="addTask">Add Task</button>
<ul id="taskList"></ul>

🧩 Requirements

✅ 1. Add Task
Take input
Create <li>
Append to list

✅ 2. Delete Task
Each task should have ❌ button
Clicking it removes ONLY that task

✅ 3. Validation
Empty input → ignore or show message

✅ 4. Add "Completed" toggle
li.addEventListener('click', () => {
    li.style.textDecoration = "line-through";
});

✅ 5. Add Edit button ✏️

✅ 6. Press Enter to add task
task.addEventListener('keypress', function(e){
    if(e.key === "Enter") add.click();
});


🧠 Skills Covered
createElement
appendChild
event inside dynamic elements
DOM structure
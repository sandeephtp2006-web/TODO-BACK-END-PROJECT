# TODO-BACK-END-PROJECT
"A simple React To-Do App using useState for managing tasks. Users can type a task, add it to the list, and delete tasks instantly. The app updates in real time, stores tasks in state, and demonstrates basic React hooks, component rendering, and event handling in a clean UI."
React To-Do App

A simple and clean To-Do application built using React. Users can add tasks, view them instantly in a list, and delete tasks with a single click. This project demonstrates core React concepts such as state management, controlled inputs, and dynamic rendering.

 Features

 Add new tasks

 Delete tasks

 Uses React useState hook

 Real-time UI updates

 Responsive and simple layout

 Project Structure
src/
│── App.js
│── index.css
│── main.jsx
└── ...

 How It Works
1. useState for Task Management
const [tasks, setTasks] = useState([]);
const [newTask, setNewTask] = useState("");


tasks stores all added tasks

newTask stores text from the input field

2. Add a Task
setTasks([...tasks, newTask]);


Adds the new task to the array

Clears the input field

3. Delete a Task
const updatedTasks = tasks.filter((_, i) => i !== index);


Removes task by index

Updates the task list

4. Rendering the Task List
tasks.map((task, index) => (
  <li key={index}>
    {task}
    <button onClick={() => deleteTask(index)}>❌</button>
  </li>
))


Loops through all tasks

Displays each with a delete button

Installation & Setup

Clone the repository

git clone https://github.com/your-username/todo-app.git


Navigate inside project

cd todo-app


Install dependencies

npm install


Run the development server

npm run dev

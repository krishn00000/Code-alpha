# ✅ Simple To-Do List

> A lightweight browser-based task manager built with **HTML, CSS, and JavaScript**. It demonstrates DOM manipulation, event handling, input validation, task completion, and task removal without requiring a framework or backend.

## 📌 Overview

The project provides a simple single-page interface for creating and managing a list of tasks directly in the browser.

Everything happens on the client side: the user enters a task, JavaScript creates the corresponding list item, and interactions update the page dynamically.

## ✨ Features

### ➕ Add a Task

The main interface contains a text field and an **Add** control.

When the user enters a task and selects **Add**:

1. JavaScript reads the value from the input field.
2. A new `<li>` element is created.
3. The entered text is inserted into the new task.
4. The task is appended to the visible list.
5. The input field is cleared for the next task.

Empty input is rejected with a browser alert so blank tasks are not added.

### ☑️ Mark a Task as Complete

Each task can be clicked to change its completion state.

The application toggles a `checked` CSS class on the selected list item. The class applies a **strikethrough effect**, giving a clear visual indication that the task has been completed.

Clicking the task again toggles the state back.

### ❌ Remove a Task

Every newly created task receives a close control represented by `×`.

Selecting the close control hides the corresponding task from the list by changing its display state. This allows unwanted tasks to be removed without refreshing the page.

### 🧹 Automatic Input Reset

After a task is processed, the input field is reset to an empty value. This keeps the interface ready for the next task and prevents accidental duplicate submission from stale input.

## 🧠 How the Interface Works

```text
User enters task
       ↓
Click Add
       ↓
Read input value
       ↓
Validate input
       ↓
Create <li>
       ↓
Add task to list
       ↓
Attach click handlers
       ↓
User can complete or remove task
```

## 🖥️ Interface

The project intentionally uses a minimal single-interface design:

### Task Input Area

- Text input for entering a task title
- Add control for creating a task

### Task List Area

- Displays all created tasks
- Clicking a task toggles completion
- `×` removes the task

There is no login system, database, backend, or separate dashboard. Tasks exist only in the current browser page and are not persisted after a page refresh.

## 🛠️ Tech Stack

- **HTML5** — page structure and task list
- **CSS3** — layout and completion styling
- **JavaScript** — DOM manipulation, validation, and interaction logic

## 🚀 Getting Started

No installation or package manager is required.

### Run Locally

1. Clone the repository:

```bash
git clone https://github.com/krishn00000/Code-alpha.git
cd Code-alpha
```

2. Open `Todolist.html` directly in a web browser.

You can also double-click the HTML file from your file explorer.

## 📁 Project Structure

```text
Code-alpha/
├── Todolist.html   # Complete application: HTML, CSS and JavaScript
└── README.md       # Project documentation
```

## 🔍 Implementation Notes

The project is intentionally framework-free. JavaScript creates and modifies DOM elements at runtime rather than relying on React, Vue, or another frontend framework.

The task lifecycle is entirely event-driven:

- **Create:** `newElement()` creates a task.
- **Complete:** clicking a task toggles the `checked` class.
- **Delete:** clicking `×` hides the parent task element.

## ⚠️ Current Limitations

- Tasks are not stored in a database.
- Tasks are not persisted in `localStorage`.
- There is no edit-task function.
- There is no task filtering or search.
- The application is intentionally a small frontend demonstration.

## 👤 Author

**Chinni Krishna Popuri**  
GitHub: [@krishn00000](https://github.com/krishn00000)

---

⭐ If you like this project, consider giving it a star.
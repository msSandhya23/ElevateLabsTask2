# ToDo CLI

Educational submission: a simple command-line To-Do list application implemented in Python.

## Purpose

This project implements a minimal interactive To-Do CLI suitable for demonstration in coursework. It supports viewing, adding, and removing tasks with persistent storage in a plain text file.

## Features

- View all tasks (numbered list)
- Add a new task
- Remove a task by index
- Persistent storage in `tasks.txt` (one task per line)

## Requirements

- Python 3.6 or newer

## Setup

1. Open PowerShell and change to the project directory:

```powershell
cd "c:\Users\sandh\OneDrive\Desktop\Task"
```

2. (Optional) Create and activate a virtual environment:

```powershell
python -m venv .venv
.venv\Scripts\Activate
```

No external dependencies are required.

## Usage

Run the application from the project directory:

```powershell
python ToDo.py
```

Interact with the menu by entering the corresponding number for each action.

Sample interaction:

```
=== TO-DO LIST MENU ===
1. View Tasks
2. Add Task
3. Remove Task
4. Exit

Enter choice: 2
Enter new task: Buy milk
Task added!

Enter choice: 1

Your Tasks:
1. Buy milk

Enter choice: 4
Goodbye! Your tasks are saved.
```

## Project files

- `ToDo.py` — source code (interactive CLI)
- `tasks.txt` — task storage (created automatically when saving tasks)

## Implementation details

The program stores tasks as plain text, one task per line. At startup, `load_tasks()` reads `tasks.txt` if present. Modifications use `save_tasks()` to overwrite the file with the current task list.

Core functions in `ToDo.py`:

- `load_tasks()`
- `save_tasks(tasks)`
- `view_tasks(tasks)`
- `add_task(tasks)`
- `remove_task(tasks)`
- `display_menu()`
- `main()` — program entrypoint and menu loop

## Submission notes

This submission is prepared for educational evaluation. Run `ToDo.py` to demonstrate functionality.

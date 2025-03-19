# Simple Todo CLI

A simple command-line todo list application built with Python and Click.

## Features

- Add new tasks to your todo list
- List all tasks with their completion status
- Mark tasks as complete
- Remove tasks from the list
- Data persists between sessions in a JSON file

## Installation

1. Clone this repository:
   ```
   git clone https://github.com/AnasAhmed001/simple-todo-cli.git
   cd simple-todo-cli
   ```

2. Install the required dependencies:
   ```
   pip install click
   ```

## Usage

The application provides several commands to manage your todo list:

### Add a task

```
python todo.py add "Your task description"
```

### List all tasks

```
python todo.py list
```

This will display all tasks with their numbers and completion status.

### Mark a task as complete

```
python todo.py complete 2
```

Replace `2` with the number of the task you want to mark as complete.

### Remove a task

```
python todo.py remove 3
```

Replace `3` with the number of the task you want to remove.

## Data Storage

All tasks are stored in a `todo.json` file in the same directory as the script. This file is created automatically when you add your first task.

## Example

```
$ python todo.py add "Buy groceries"
Added task: Buy groceries

$ python todo.py add "Finish homework"
Added task: Finish homework

$ python todo.py list
1. [ ] Buy groceries
2. [ ] Finish homework

$ python todo.py complete 1
Completed task: Buy groceries

$ python todo.py list
1. [x] Buy groceries
2. [ ] Finish homework

$ python todo.py remove 1
Removed task: Buy groceries

$ python todo.py list
1. [ ] Finish homework
```

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.


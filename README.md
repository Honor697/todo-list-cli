# Todo List CLI

A simple command-line to-do list application built with Node.js that helps you manage your tasks efficiently.

## Features

- Add new tasks
- View pending tasks
- Mark tasks as completed
- Delete tasks
- View task statistics and reports

## Installation

1. Clone this repository
2. Navigate to the project directory
3. Run the application using Node.js

## Usage

```bash
# Add a new todo
$ node index.js add "todo item"

# Show remaining todos
$ node index.js ls

# Delete a todo
$ node index.js del NUMBER

# Complete a todo
$ node index.js done NUMBER

# Show usage help
$ node index.js help

# View statistics
$ node index.js report
```

## How It Works

The application stores tasks in two files:
- `todo.txt` - Contains pending tasks
- `done.txt` - Contains completed tasks with completion dates

When you mark a task as done, it's moved from `todo.txt` to `done.txt` with a timestamp.

## Examples

### Adding a task
```bash
$ node index.js add "Buy groceries"
Added todo: "Buy groceries"
```

### Viewing all tasks
```bash
$ node index.js ls
1. Buy groceries
2. Finish homework
3. Call dentist
```

### Completing a task
```bash
$ node index.js done 1
Marked todo #1 as done.
```

### Deleting a task
```bash
$ node index.js del 2
Deleted todo #2
```

### Viewing report
```bash
$ node index.js report
2025-10-25 Pending : 2 Completed : 1
```

## Requirements

- Node.js (version 12 or higher)

## License

ISC

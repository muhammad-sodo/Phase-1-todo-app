# Quickstart Guide: Console Todo Application

**Date**: 2026-01-02
**Feature**: Console Todo Application
**Branch**: 001-console-todo

## Getting Started

This guide will help you set up and run the console todo application.

### Prerequisites

- Python 3.13 or higher
- pip package manager

### Setup

1. **Clone or create the project structure**:
   ```
   todo-app/
   ├── src/
   │   ├── models/
   │   ├── services/
   │   ├── cli/
   │   └── lib/
   └── tests/
   ```

2. **Create the main application files** based on the architecture:
   - `src/models/task.py` - Task entity
   - `src/services/todo_service.py` - Business logic
   - `src/cli/todo_cli.py` - Command-line interface
   - `src/lib/storage.py` - In-memory storage

### Running the Application

1. **Execute the CLI application**:
   ```bash
   python -m src.cli.todo_cli
   ```

2. **Use the menu options**:
   - Add a new task
   - View all tasks
   - Update a task
   - Complete a task
   - Delete a task
   - Exit the application

### Basic Usage

1. **Adding a task**: Select option to add a task and enter the description
2. **Viewing tasks**: Select option to see all tasks with their status
3. **Updating tasks**: Select option to update with task ID and new description
4. **Completing tasks**: Select option to mark a task as complete
5. **Deleting tasks**: Select option to remove a task by ID

### Running Tests

Execute the test suite to verify functionality:

```bash
# Run all tests
python -m pytest tests/

# Run specific test categories
python -m pytest tests/unit/
python -m pytest tests/integration/
```

### Configuration

The application runs with default settings. No configuration file is needed as all storage is in-memory only.
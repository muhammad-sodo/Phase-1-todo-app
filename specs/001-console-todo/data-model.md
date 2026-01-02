# Data Model: Console Todo Application

**Date**: 2026-01-02
**Feature**: Console Todo Application
**Branch**: 001-console-todo

## Task Entity

### Attributes
- **id**: Unique identifier (string or integer) - automatically generated
- **description**: Task description (string) - required, non-empty
- **status**: Completion status (string) - values: "pending", "complete"
- **created_at**: Creation timestamp (datetime) - automatically set

### Validation Rules
- Description must not be empty or null
- ID must be unique within the application session
- Status must be one of the allowed values
- Creation timestamp automatically set on creation

### State Transitions
- Initial state: "pending"
- Transitions: "pending" ↔ "complete" (bidirectional)
- No other state transitions allowed

### Relationships
- No relationships with other entities (standalone entity)

## In-Memory Storage Model

### Storage Structure
- **tasks**: Dictionary where key = task ID, value = Task object
- **next_id**: Integer counter for generating unique IDs

### Operations
- **Create**: Add new task to dictionary with unique ID
- **Read**: Retrieve task by ID from dictionary
- **Update**: Modify existing task properties in dictionary
- **Delete**: Remove task from dictionary by ID
- **List**: Return all tasks from dictionary
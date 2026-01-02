# API Contracts: Console Todo Application

**Date**: 2026-01-02
**Feature**: Console Todo Application
**Branch**: 001-console-todo

## Overview

This document defines the functional contracts for the console todo application. Since this is a command-line application without a traditional API, these contracts define the expected behavior and interfaces of the core services.

## Todo Service Contract

### Add Task
- **Input**: Task description (string)
- **Output**: Task object with ID, description, status="pending", created_at
- **Preconditions**: Description is not empty
- **Postconditions**: Task exists in storage with unique ID
- **Error cases**: Empty description returns error message

### List Tasks
- **Input**: None
- **Output**: Array of Task objects
- **Preconditions**: None
- **Postconditions**: Returns all tasks in storage
- **Error cases**: None

### Update Task
- **Input**: Task ID (string/integer), updated description (string)
- **Output**: Updated Task object
- **Preconditions**: Task exists with given ID
- **Postconditions**: Task description updated in storage
- **Error cases**: Task ID not found returns error message

### Complete Task
- **Input**: Task ID (string/integer)
- **Output**: Updated Task object with status="complete"
- **Preconditions**: Task exists with given ID
- **Postconditions**: Task status updated to "complete"
- **Error cases**: Task ID not found returns error message

### Delete Task
- **Input**: Task ID (string/integer)
- **Output**: Success confirmation or error message
- **Preconditions**: Task exists with given ID
- **Postconditions**: Task removed from storage
- **Error cases**: Task ID not found returns error message

### Get Task
- **Input**: Task ID (string/integer)
- **Output**: Task object or error message
- **Preconditions**: Task exists with given ID
- **Postconditions**: Returns specific Task object
- **Error cases**: Task ID not found returns error message
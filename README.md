# Todo App API

This repository contains the backend code for a simple Todo App API implemented in Java using the Spring Boot framework. The API provides endpoints for managing todo items.

## Table of Contents

- [Controller](#controller)
- [Endpoints](#endpoints)

## Controller

### TodoController

#### `addTodo`

- **Endpoint:** `POST /todo`
- **Description:** Adds a new todo item to the list.
- **Request Body:**
  - `Todo`: Todo details to be added.
- **Response:** Returns a message indicating the success of the todo addition.

#### `getAllTodos`

- **Endpoint:** `GET /todos`
- **Description:** Retrieves all todo items from the list.
- **Response:** Returns a list of all todo items.

#### `setTodoStatusById`

- **Endpoint:** `PUT /todo/id/{id}/status`
- **Description:** Updates the status of a todo item by ID.
- **Path Variables:**
  - `id`: ID of the todo item.
- **Request Parameters:**
  - `flag`: New status for the todo item.
- **Response:** Returns a message indicating the success of the todo status update.

#### `removeTodoById`

- **Endpoint:** `DELETE /todo/id/{id}`
- **Description:** Removes a todo item by ID.
- **Path Variables:**
  - `id`: ID of the todo item.
- **Response:** Returns a message indicating the success of the todo removal.


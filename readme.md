# CRUD React Go Project

This project is a simple Todo application demonstrating a CRUD (Create, Read, Update, Delete) API built with Go (Golang), Fiber web framework, and MongoDB as the database. The backend serves a RESTful API for managing todo items. The project is designed to be paired with a React frontend (not included here).

## Features
- RESTful API for Todo items
- MongoDB integration
- Environment variable support via `.env`
- Example endpoints for listing, creating, updating, and deleting todos

## Prerequisites
- Go 1.18+
- MongoDB instance (local or cloud)
- Node.js & npm (for React frontend, not included)

## Getting Started

### 1. Clone the repository
```sh
git clone <repo-url>
cd crud-react-go
```

### 2. Set up environment variables
Create a `.env` file in the root directory with the following content:
```
MONGO_DB_URI=mongodb://localhost:27017
PORT=3000
```
Adjust the values as needed for your MongoDB setup and desired port.

### 3. Install Go dependencies
```sh
go mod tidy
```

### 4. Run the server
```sh
go run main.go
```
The server will start on the port specified in your `.env` file (default: 3000).

## API Endpoints
- `GET /api/todos` - List all todos
- `POST /api/todos` - Create a new todo *(to be implemented)*
- `PATCH /api/todos/:id` - Update a todo *(to be implemented)*
- `DELETE /api/todos/:id` - Delete a todo *(to be implemented)*

## Project Structure
```
crud-react-go/
├── main.go                # Go backend source code
├── go.mod, go.sum         # Go module files
├── air.toml               # (Optional) Air config for live reloading
├── react-go-crud.postman_collection.json # Postman collection for API testing
├── tmp/                   # Temporary build/output files
```

## Testing the API
Use the provided Postman collection (`react-go-crud.postman_collection.json`) to test the API endpoints.

## License
MIT

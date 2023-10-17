
# Todo App with CRUD Operations

## Frameworks and Language Used

- Database: MongoDB
- Language: Java

## Data Flow

### Controller
The controller layer of our application is responsible for handling incoming HTTP requests, processing them, and sending appropriate responses. It utilizes the following functions:

- `createTodo`: Handles the creation of new todo items.
- `getTodo`: Retrieves information about a specific todo item.
- `updateTodo`: Allows for updating todo item details.
- `deleteTodo`: Deletes a todo item from the system.
- `getAllTodos`: Fetches a list of all todo items.

### Services
The services layer acts as an intermediary between the controller and the repository. It encapsulates the business logic and performs data validation. It includes the following functions:

- `validateTodoData`: Validates the todo item data before saving it.
- `formatTodoResponse`: Formats the todo item data before sending it to the client.
- `sendTodoUpdateNotification`: Sends notifications when a todo item is updated.

### Repository
The repository layer handles database operations and interactions with our MongoDB database. It provides the following functions:

- `createTodo`: Saves todo item data to the database.
- `findTodoById`: Retrieves a todo item by its unique ID.
- `updateTodoData`: Updates todo item details in the database.
- `deleteTodoById`: Deletes a todo item from the database.
- `findAllTodos`: Retrieves all todo items from the database.

## Database Design

We use MongoDB as our database, organizing data in a collection named `todos`. Each document in the collection represents a todo item and includes fields like title, description, status, and timestamps for creation and modification.

## Data Structures Used

- JSON: We use JSON objects for data representation and transmission in API requests and responses.
- NoSQL Database: Our application leverages MongoDB, a NoSQL database, to store and query todo item data efficiently.

## Project Summary

The Todo App with CRUD Operations is built MongoDB serves as the database, and the application provides features for creating, managing, and viewing todo items. The system is designed to ensure seamless data management and user-friendly todo item updates. It aims to help users organize their tasks effectively and efficiently through a user-friendly interface.

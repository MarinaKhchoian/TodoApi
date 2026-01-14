# TodoAp
Todo List API

A simple REST API for managing a Todo List.
This project is built with ASP.NET Core Web API and Entity Framework Core.

Technologies
ASP.NET Core Web API

Entity Framework Core (InMemory Database)
C#
.NET 6+
Features

The API supports basic CRUD operations:

GET /api/todo – get all todo items
GET /api/todo/{id} – get a todo item by id
POST /api/todo – create a new todo item
PUT /api/todo/{id} – update an existing todo item
DELETE /api/todo/{id} – delete a todo item


Data Model
public class TodoItem
{
    public int Id { get; set; }
    public string Title { get; set; }
    public string Description { get; set; }
    public bool IsCompleted { get; set; }
    public DateTime CreatedAt { get; set; }
}

How to Run the Project

Clone the repository
Open the project in Visual Studio 2022
Press F5 to run the project
Swagger UI will open in the browser to test the API


Example Requests
Create a Todo (POST)
{
  "title": "Learn ASP.NET Core",
  "description": "Complete Web API tutorial",
  "isCompleted": false
}

Update a Todo (PUT)
{
  "id": 1,
  "title": "Learn ASP.NET Core",
  "description": "Complete Web API tutorial",
  "isCompleted": true,
  "createdAt": "2024-01-15T10:00:00"
}

What I Learned

While working on this project, I learned how to:
Build APIs with ASP.NET Core Web API
Use Entity Framework Core to work with data
Follow REST principles
Implement CRUD operations
Use async and await for asynchronous programming


Future Improvements
 Use a real database (SQL Server)
 Add data validation
 Add JWT authentication
 Add unit tests
 Add pagination for the todo list

Author Marina Khchoian
This project was created as part of learning .NET development and preparing for an internship.

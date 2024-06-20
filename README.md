# TodoApp

Endpoints:

AuthController.cs
This controller handles user authentication.

1. POST /api/auth/register
	•	Description: Registers a new user.
	•	Request Body:
{
  "Username": "string",
  "Email": "string",
  "Password": "string"
}

2.	POST /api/auth/login
	•	Description: Logs in an existing user.
	•	Request Body:
{
  "Username": "string",
  "Password": "string"
}


TodoItemsController.cs

This controller handles operations related to Todo items.

Endpoints:

1.	GET /api/todoitems
	•	Description: Retrieves all todo items.
	•	No request body or parameters required.
	 
	
2.	GET /api/todoitems/{id}
	•	Description: Retrieves a single todo item by ID.
	•	Parameters:
	•	id (int): The ID of the todo item.
	
	
3.	POST /api/todoitems
	•	Description: Creates a new todo item.
	•	Request Body:
{
  "Name": "string",
  "IsComplete": "boolean"
}
	

4.	PUT /api/todoitems/{id}
	•	Description: Updates an existing todo item by ID.
	•	Parameters:
	•	id (int): The ID of the todo item.
	•	Request Body:
{
  "Id": "int",
  "Name": "string",
  "IsComplete": "boolean"
}
	

5.	DELETE /api/todoitems/{id}
	•	Description: Deletes a todo item by ID.
	•	Parameters:
	•	id (int): The ID of the todo item.
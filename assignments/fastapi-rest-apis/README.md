# 📘 Assignment: Building REST APIs with FastAPI

## 🎯 Objective

Build a fully functional REST API using FastAPI framework to handle CRUD operations on a resource. Learn how to create endpoints, implement request/response models, handle errors, and test your API. You'll practice building scalable web services and understand modern API design principles.

## 📝 Tasks

### 🛠️ Project Setup and Basic Endpoint

#### Description
Set up a FastAPI project and create your first endpoint that responds to HTTP requests with JSON data.

#### Requirements
Completed program should:

- Install FastAPI and Uvicorn using pip
- Create a main application file using `FastAPI()`
- Implement a GET endpoint at `/` that returns a welcome message
- Run the development server using `uvicorn main:app --reload`
- Verify the endpoint is accessible at `http://localhost:8000`

### 🛠️ Create Data Models with Pydantic

#### Description
Define request and response data models using Pydantic to ensure type safety and automatic validation.

#### Requirements
Completed program should:

- Create a Pydantic model for your resource (e.g., `Item`, `User`, `Post`)
- Include at least 3 fields with appropriate data types
- Add field validation using Pydantic validators
- Use the model in your API responses
- Example model:
  ```python
  from pydantic import BaseModel
  
  class Item(BaseModel):
      id: int
      name: str
      price: float
      description: str = None
  ```

### 🛠️ Implement CRUD Endpoints

#### Description
Create endpoints to perform Create, Read, Update, and Delete operations on your resource.

#### Requirements
Completed program should:

- Implement `GET /items` to retrieve all items
- Implement `GET /items/{item_id}` to retrieve a single item by ID
- Implement `POST /items` to create a new item
- Implement `PUT /items/{item_id}` to update an existing item
- Implement `DELETE /items/{item_id}` to delete an item
- Store data in a list or dictionary (in-memory database)
- Return appropriate HTTP status codes (200, 201, 404, etc.)

### 🛠️ Error Handling and Validation

#### Description
Add proper error handling and request validation to make your API robust and user-friendly.

#### Requirements
Completed program should:

- Validate request data using Pydantic models
- Return 404 Not Found when accessing non-existent items
- Return 400 Bad Request for invalid input data
- Return 422 Unprocessable Entity for validation errors
- Include error messages in response JSON
- Example error response:
  ```json
  {
    "detail": "Item not found"
  }
  ```

### 🛠️ API Documentation and Testing

#### Description
Generate interactive API documentation and test all endpoints to ensure they work correctly.

#### Requirements
Completed program should:

- Access auto-generated Swagger UI documentation at `/docs`
- Access ReDoc documentation at `/redoc`
- Test all CRUD endpoints using the interactive documentation
- Verify proper request and response formats
- Test edge cases (missing fields, invalid IDs, etc.)
- Document any custom behavior or business logic

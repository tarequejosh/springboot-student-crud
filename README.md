# Spring Boot Student Management CRUD

A simple beginner-friendly Spring Boot project for managing students with MySQL database.

## Features
- Add, view, update, and delete students
- Simple REST API
- Uses MySQL for data storage

## Setup
1. **Clone the repository:**
   ```sh
   git clone https://github.com/tarequejosh/springboot-student-crud.git
   cd springboot-student-crud
   ```
2. **Configure MySQL:**
   - Make sure MySQL is running.
   - Create a database named `studentDatabase`.
   - Update `src/main/resources/application.properties` with your MySQL username and password.
3. **Build and run the project:**
   ```sh
   ./mvnw spring-boot:run
   ```

## API Endpoints
| Method | Endpoint                     | Description            |
|--------|-------------------------------|------------------------|
| GET    | `/students`                   | Get all students       |
| GET    | `/student/{id}`               | Get student by ID      |
| POST   | `/student/add`                | Add a new student      |
| PUT    | `/student/update/{id}`        | Update a student       |
| DELETE | `/student/delete/{id}`        | Delete a student       |

## Example Student JSON
```json
{
  "name": "Tareque Josh",
  "email": "tareque@example.com",
  "department": "Computer Science",
  "percentage": "85"
}
```

## Testing
- Use [Postman](https://www.postman.com/downloads/) or similar tool to test the endpoints.

## Notes
- This project is intentionally simple for learning purposes.
- No authentication or advanced error handling is included. 
# Employee Management System

A full-stack web application for managing employee information, built with Spring Boot and React.

## Features

- Create, Read, Update, and Delete (CRUD) employee records
- Modern and responsive user interface
- RESTful API architecture
- In-memory H2 database for data persistence
- Real-time data updates

## Tech Stack

### Backend
- Java 17
- Spring Boot 3.2.3
- Spring Data JPA
- H2 Database
- Lombok
- Maven

### Frontend
- React.js
- Axios for API calls
- Bootstrap for styling
- React Router for navigation

## Prerequisites

- Java JDK 17 or higher
- Node.js and npm
- Maven

## Getting Started

### Backend Setup

1. Navigate to the backend directory:
   ```bash
   cd Backend
   ```

2. Run the Spring Boot application:
   ```bash
   ./mvnw spring-boot:run
   ```

The backend server will start at `http://localhost:8080`

### Frontend Setup

1. Navigate to the frontend directory:
   ```bash
   cd Frontend/employee_management
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   npm start
   ```

The frontend application will start at `http://localhost:3000`

## API Endpoints

- `GET /api/employees` - Get all employees
- `GET /api/employees/{id}` - Get employee by ID
- `POST /api/employees` - Create new employee
- `PUT /api/employees/{id}` - Update employee
- `DELETE /api/employees/{id}` - Delete employee

## Database Configuration

The application uses H2 in-memory database with the following configuration:
- JDBC URL: `jdbc:h2:mem:employeedb`
- Username: `sa`
- Password: (empty)
- H2 Console: `http://localhost:8080/h2-console`

## Project Structure

```
ems/
├── Backend/                 # Spring Boot backend
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/       # Java source files
│   │   │   └── resources/  # Configuration files
│   │   └── test/           # Test files
│   └── pom.xml             # Maven dependencies
│
└── Frontend/               # React frontend
    └── employee_management/
        ├── src/            # React source files
        ├── public/         # Static files
        └── package.json    # npm dependencies
```

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.
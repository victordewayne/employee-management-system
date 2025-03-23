# Employee Management System (Spring Boot + MySQL)

This is a simple Employee Management System built using Spring Boot, Spring Data JPA, and MySQL.

# Features
- Create, Read, Update, and Delete (CRUD) employees
- RESTful API using Spring Boot
- MySQL database integration

# Technologies Used
- Java 17
- Spring Boot
- Spring Data JPA
- MySQL
- Maven
- Lombok

## Setup and Installation

# 1. Clone the Repository
```sh
git clone https://github.com/yourusername/employee-management-system.git
cd employee-management-system
```

# 2️. Configure MySQL Database
Create a database named `employeedb` in MySQL and update `application.properties`:
properties
spring.datasource.url=jdbc:mysql://localhost:3306/employeedb
spring.datasource.username=root
spring.datasource.password=your_mysql_password

# 3. Run the Application
mvn spring-boot:run


# API Endpoints

# Create Employee (POST)

curl -X POST http://localhost:8080/employees -H "Content-Type: application/json" -d "{\"name\":\"John Doe\", \"role\":\"Software Engineer\", \"salary\":75000}"

# Get All Employees (GET)

curl -X GET http://localhost:8080/employees

# Get Employee by ID (GET)

curl -X GET http://localhost:8080/employees/1

# Update Employee (PUT)

curl -X PUT http://localhost:8080/employees/1 -H "Content-Type: application/json" -d "{\"name\":\"John Doe\", \"role\":\"Senior Engineer\", \"salary\":90000}"

# Delete Employee (DELETE)

curl -X DELETE http://localhost:8080/employees/1





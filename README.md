# Spring Boot REST API - Student Management

## Project Overview
This Spring Boot REST API manages student information. It provides endpoints to retrieve, filter, sort, and perform CRUD operations on student records.

## Project Structure
- **AppController.java** - Main REST controller with endpoints for student operations.
- **Student.java** - Model class representing student attributes.



## Prerequisites
- Java 8 or higher
- Spring Boot
- Maven or Gradle

## Dependencies
- Spring Web
- Spring Data JPA



## Endpoints

### 1. Display Age
- **URL:** `/app/age`
- **Method:** `GET`
- **Response:** "My age is: 32"

### 2. Get a Single Student
- **URL:** `/app/student`
- **Method:** `GET`
- **Description:** Returns a single predefined student.

### 3. Get Multiple Students
- **URL:** `/app/students`
- **Method:** `GET`
- **Description:** Returns a list of all predefined students.

### 4. Find a Student by Registration Number
- **URL:** `/app/students/{regNo}`
- **Method:** `GET`
- **Description:** Returns a specific student based on the registration number.
- **Example:** `/app/students/2020ICT47`

### 5. Find Students by Age Range (20-24)
- **URL:** `/app/students/age`
- **Method:** `GET`
- **Description:** Returns students whose age is between 20 and 24.

### 6. Sort Students by GPA
- **URL:** `/app/students/gpa`
- **Method:** `GET`
- **Description:** Returns students sorted by GPA in ascending order.

### 7. CRUD Operations

#### Create Student
- **URL:** `/app/students`
- **Method:** `POST`
- **Description:** Adds a new student.
- **Request Body Example:**
```json
{
  "regNo": "2020ICT01",
  "name": "Bingu Sala",
  "age": 24,
  "course": "ICT",
  "gpa": 3.8
}
```

#### Update Student
- **URL:** `/app/students/{regNo}`
- **Method:** `PUT`
- **Description:** Updates student details based on the registration number.

#### Delete Student
- **URL:** `/app/students/{regNo}`
- **Method:** `DELETE`
- **Description:** Deletes a student by registration number.

## Student Model
The `Student` class has the following attributes:
- `regNo` - Registration Number (String)
- `name` - Student Name (String)
- `age` - Student Age (Integer)
- `course` - Student's Course (String)
- `gpa` - Student's Grade Point Average (Double)

## Running the Application
1. Ensure you have Java and Spring Boot installed.
2. Clone the repository.
3. Build the project using Maven or Gradle.
4. Run the Spring Boot application.
5. Access endpoints via `http://localhost:8080/app/...`

## Outputs
1. **Welcome Message:**
   - Screenshot (969)
2. **Age Endpoint:**
   - Screenshot (970)
3. **Get Single Student:**
   - Screenshot (971)
4. **Get All Students:**
   - Screenshot (972, 973)
5. **Find Student by RegNo:**
   - Screenshot (978)
6. **Find Students by Age (20-24):**
   - Screenshot (975)
7. **Sorted Students by GPA:**
   - Screenshot (976, 977)





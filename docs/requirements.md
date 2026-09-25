# Customizable Academic Management API

## Objective

Build a REST API that allows a university or organization to configure and manage its academic structure without modifying the application source code.

## Core Requirements

### University
- Create university
- Update university
- Delete university
- Get university

### Degree
- A university can have multiple degrees
- Example: B.Tech, BCA, B.Sc
- Degree belongs to a university

### Curriculum
- A degree can have multiple curriculum/schemes
- Example: 2021 Scheme, 2022 Scheme, 2026 Scheme
- Curriculum belongs to a degree

### Courses
- Create courses
- Update courses
- Delete courses
- Get courses
- Course has:
  - Id
  - Name
  - Code
  - Credits

### Curriculum Courses
A curriculum determines which courses are offered.

Each curriculum course should contain:
- Course
- Semester
- Mandatory/Optional

This allows different schemes to have different course structures.

### Students
Student should have:
- Id
- First Name
- Last Name
- Email
- Roll Number
- Curriculum

### Student Enrollment
Students can enroll in courses.

Rules:
- A student cannot enroll in the same course twice
- A student should only enroll in courses available in their curriculum

### Professors
Professor should have:
- Id
- Name
- Employee Id
- Email

### Teaching Assignment
Professors can be assigned to courses.

## Technical Requirements

- C#
- .NET
- ASP.NET Core Web API
- Entity Framework Core
- SQL Server
- REST API
- Git/GitHub
- Postman
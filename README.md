# Student Management Dashboard (Frontend)

This repository contains the **frontend dashboard** for the Student Management System.
It connects to a FastAPI backend to perform CRUD operations on student records.

## Features

* Login with JWT authentication
* View all students
* Add new student
* Edit student information
* Delete student
* Dashboard statistics (Total Students & Average Age)
* FastAPI REST API integration

## Tech Stack

* HTML
* CSS
* JavaScript
* Bootstrap

## Project Structure

```
frontend
│
├── index.html
├── login.html
├── script.js
├── api_helper.js
└── style.css
```

## How It Works

1. User logs in using credentials.
2. Backend returns a JWT token.
3. Token is stored in browser localStorage.
4. All API requests include the token in Authorization headers.
5. The dashboard communicates with the FastAPI backend.

Example API call:

```
GET /students/
Authorization: Bearer <token>
```

## Running the Frontend

1. Start the FastAPI backend.

```
uvicorn main:app --reload
```

2. Open the frontend using **Live Server**.

```
index.html
```

## Backend Repository

The backend API is available here:

https://github.com/yourusername/student-management-backend

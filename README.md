# API-Documentation-Sample
This document provides a sample API documentation for creating a new user, including detailed request and response examples formatted in JSON.

## Overview
The Create User API provides endpoints for creating user accounts in your application.
Designed for easy integration, this API supports JSON requests and responses,
ensuring seamless communication between front-end and back-end components.

### Create User
Endpoint: `POST /api/users`

Description: Creates a new user account.

Request Headers:
```
Content-Type: application/json
Authorization: Bearer <token>
```

#### Request Body:

```
{
  "username": "john_doe",
  "email": "john@example.com",
  "password": "securepassword123",
  "firstName": "John",
  "lastName": "Doe"
}
```
#### Response:
Status Code: `201 Created`
##### Body:
```
{
  "id": "12345",
  "username": "john_doe",
  "email": "john@example.com",
  "firstName": "John",
  "lastName": "Doe",
  "createdAt": "2024-09-03T12:00:00Z"
}
```
#### Error Responses:
Status Code: `400 Bad Request`
```
{
  "error": "Invalid input data"
}
```
This example illustrates document API endpoints, including the request and response structures, headers, parameters, and error handling to ensure comprehensive and user-friendly API documentation.

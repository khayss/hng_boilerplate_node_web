# HNG Boilerplate API

## Overview

The HNG Boilerplate API provides a simple, secure, and efficient way to manage user accounts and organizations. This API follows the OpenAPI specification for documentation and includes user authentication, organization management, and user settings.

## Features

- User authentication (signup, login, password reset)
- User profile management
- Organization creation and membership management
- JWT-based authentication
- Activity logging and notification settings

## API Endpoints

### Authentication

- **POST /auth/signup**: Create a new account
- **POST /auth/login**: Sign in to the account
- **POST /auth/forgot-password**: Initiate password reset process
- **POST /auth/reset-password**: Reset user password
- **GET /auth/profile**: Get user details (protected route)

### User Management

- **PUT /users/{id}**: Update user profile (protected route)
- **GET /users/{id}**: Get specific user details (protected route)
- **GET /users/{id}/settings**: Retrieve user-specific settings (protected route)
- **PUT /users/{id}/settings**: Update user-specific settings (protected route)
- **GET /users/{id}/activity**: Retrieve a user's activity log (protected route)

### Organization Management

- **POST /organizations**: Create a new organization (protected route)
- **GET /organizations/{id}**: Get organization details (protected route)
- **PUT /organizations/{id}**: Update organization details (protected route)
- **DELETE /organizations/{id}**: Delete an organization (protected route)
- **POST /organizations/{id}/members**: Add members to an organization (protected route)
- **DELETE /organizations/{id}/members/{userId}**: Remove a member from an organization (protected route)
- **GET /organizations/{id}/members**: Get members of an organization (protected route)
- **GET /organizations/search**: Search for organizations (public)

## Database Design

The database includes the following tables:

- **Users**: Stores user details and authentication information.
- **Organizations**: Contains organization information.
- **Organization Members**: Manages user memberships in organizations.
- **Settings**: Stores user-specific settings.
- **Notifications**: Handles notifications for users.
- **User Activity**: Logs user activities for auditing.
- **Database Design**: The database design is store an image in the root directory (db_design.jpeg).

## Setup Instructions

1. Clone the repository:
   ```bash
   git clone https://github.com/khayss/hng_boilerplate_node_web.git

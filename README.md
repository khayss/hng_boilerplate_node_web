# HNG Boilerplate API - Users

This section describes the API endpoints related to user management in the HNG Boilerplate API.

## Users API Endpoints

### 1. Retrieve User Profile
- **Endpoint:** `GET /users/{id}/profile`
- **Description:** Retrieve user profile information.
- **Security:** Requires Bearer Token
- **Responses:**
  - `200`: User profile retrieved successfully.
  - `404`: User not found.

---

### 2. Deactivate User Account
- **Endpoint:** `POST /users/{id}/deactivate`
- **Description:** Deactivate a user account.
- **Security:** Requires Bearer Token
- **Responses:**
  - `204`: User account deactivated successfully.
  - `404`: User not found.

---

### 3. Reactivate User Account
- **Endpoint:** `POST /users/{id}/reactivate`
- **Description:** Reactivate a deactivated user account.
- **Security:** Requires Bearer Token
- **Responses:**
  - `204`: User account reactivated successfully.
  - `404`: User not found.

---

### 4. Get User Notifications
- **Endpoint:** `GET /users/{id}/notifications`
- **Description:** Get user notifications.
- **Security:** Requires Bearer Token
- **Responses:**
  - `200`: User notifications retrieved successfully.

---

### 5. Retrieve User Settings
- **Endpoint:** `GET /users/{id}/settings`
- **Description:** Retrieve user-specific settings.
- **Security:** Requires Bearer Token
- **Responses:**
  - `200`: User settings retrieved successfully.

### 6. Update User Settings
- **Endpoint:** `PUT /users/{id}/settings`
- **Description:** Update user-specific settings.
- **Security:** Requires Bearer Token
- **Request Body:**
```json
{
    "setting_key": "string",
    "setting_value": "string"
}
F
- **Database Design**
  The database design is store an image in the root directory (db_design.jpeg).

## API Documentation

The API follows the OpenAPI specification. You can view the interactive documentation and test endpoints using the link below.
[Documentation](https://test002.otecfx.com/documentation/#/)


## Setup Instructions

1. Clone the repository:
   ```bash
   git clone https://github.com/khayss/hng_boilerplate_node_web.git

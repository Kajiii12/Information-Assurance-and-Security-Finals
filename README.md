# Plan and Done

## Overview
Plan and Done is a Task Management system. It is a web-based platform built using Flask for managing users, their profiles, and administrative functions. It offers secure user authentication, role-based access control, and profile management. The application integrates with a SQLite3 database, allowing admins to manage user accounts effectively.

---

## Features

- **User Authentication**:
  - Secure login and registration.
  - Password hashing using SHA-256.
- **Role-Based Access Control**:
  - Admin-specific features such as managing users.
  - Protected routes for authenticated users.
- **Profile Management**:
  - Users can add profile pictures.
- **File Uploads**:
  - Support for profile picture uploads (PNG, JPG, JPEG).
  - File size limit of 5 MB.
- **Admin Functionalities**:
  - Add, edit, and delete users.
  - View a list of all users.

---

## Security Features

- **Password Hashing**:
  - User passwords are hashed with SHA-256 before storing in the database.
- **Role-Based Access**:
  - Admin-only routes are protected with a decorator (`@admin_required`).
  - User-only routes require authentication (`@login_required`).
- **Session Management**:
  - Sessions are secured with a secret key and have a defined lifetime.

---

## Prerequisites

- Python 3.7+
- SQLite3 Database

---

## Usage

1. **Login**:
   - Access the login page at `/login`.
   - Admins can log in to access user management features.

2. **User Management (Admin Only)**:
   - View all users at `/users`.
   - Add a new user at `/add_user`.
   - Edit user details at `/edit_user/<user_id>`.
   - Delete a user via the delete button on the users list page.

3. **Profile Management**:
   - Capture a live image for profile picture

4. **Logout**:
   - Log out using the `/logout` endpoint.

---

## Folder Structure

```
├── add.py               # Migration Script
├── refactor kuno    
    └──  app.py          # Main Program
    ├──static            # CSS templates
       └── avatars/      # Profile Pictures
    ├──templates/        # HTML Templates
├── todo_app.db          # Database
```

## Future Enhancements

- Advanced Task Management Features.
- Enhanced Security.
- Performance Optimization.
- Improved User Experience.

---

## License

This project is licensed under the MIT License. See the LICENSE file for details.

---

## Contributing

Contributions are welcome! Please submit a pull request or open an issue to propose changes.

---

## Contact

For questions or support, please contact:

- **Name**: [Joshua Ean C. Valera]
- **Email**: [jovalera@my.cspc.edu.ph]
- **GitHub**: [https://github.com/Joshua-Ean-Valera]

- **Name**: [Mary Rachel Parañal]
- **Email**: [maparanal@my.cspc.edu.ph]
- **GitHub**: [https://github.com/xxrachelpxx]

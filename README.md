# EmployWise React Assignment

## Overview
This is a React application that integrates with the [Reqres API](https://reqres.in/) to perform basic user management functions, including authentication, listing users, editing user details, and deleting users.

## Features
### Level 1: Authentication Screen
- Users can log in using the following credentials:
  - **Email:** eve.holt@reqres.in
  - **Password:** cityslicka
- Token received upon successful login is stored in `localStorage`.
- On successful login, users are redirected to the **Users List** page.

### Level 2: List All Users
- Fetches users from `GET /api/users?page=1`.
- Displays user details in a card layout.
- Implements pagination for navigating between user pages.

### Level 3: Edit, Delete, and Update Users
- **Edit User:**
  - Clicking **Edit** opens a form pre-filled with user data.
  - Users can update first name, last name, and email.
  - Uses `PUT /api/users/{id}` for updates.
- **Delete User:**
  - Clicking **Delete** removes the user from the list.
  - Uses `DELETE /api/users/{id}` for deletion.

### Additional Features
- React Router for navigation.
- Error handling for API failures.
- Client-side search and filtering.
- Hosted on **Vercel/Netlify**.

## Tech Stack
- **Frontend:** React (Vite)
- **State Management:** useState, useEffect
- **HTTP Requests:** Axios
- **Routing:** React Router
- **Styling:** Tailwind CSS
- **Persistence:** LocalStorage for token storage

## Installation and Setup
1. **Clone the repository**
   ```sh
   git clone https://github.com/your-username/employwise-assignment.git
   cd employwise-assignment
   ```
2. **Install dependencies**
   ```sh
   npm install
   ```
3. **Run the development server**
   ```sh
   npm start
   ```
4. **Build for production**
   ```sh
   npm run build
   ```

## API Endpoints Used
| Action         | Method | Endpoint             |
|---------------|--------|----------------------|
| Login         | POST   | `/api/login`         |
| Fetch Users   | GET    | `/api/users?page=1`  |
| Update User   | PUT    | `/api/users/{id}`    |
| Delete User   | DELETE | `/api/users/{id}`    |

## Deployment
The application is hosted on **[Vercel/Netlify](https://your-live-link.com)**.

## Folder Structure
```
📦 employwise-assignment
 ┣ 📂 src
 ┃ ┣ 📂 components
 ┃ ┃ ┣ 📜 LoginForm.jsx
 ┃ ┃ ┣ 📜 UserList.jsx
 ┃ ┃ ┣ 📜 EditUserModal.jsx
 ┃ ┣ 📂 pages
 ┃ ┃ ┣ 📜 Login.jsx
 ┃ ┃ ┣ 📜 Users.jsx
 ┃ ┣ 📂 services
 ┃ ┃ ┣ 📜 api.js
 ┃ ┣ 📜 App.jsx
 ┃ ┣ 📜 index.js
 ┣ 📜 package.json
 ┣ 📜 README.md
```

## Future Enhancements
- Implement **JWT authentication**.
- Add **unit tests** for key components.
- Improve UI with **Material-UI**.



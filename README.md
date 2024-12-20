
## Book Center

Book Center is a comprehensive and user-friendly web designed to facilitate book management and access for students, faculty, and staff. The system provides tailored functionalities for each user role, ensuring an efficient and engaging experience.

## Features

### Student

- **Account Management**: Register, log in, view
- **Book Interaction**:
  - Browse available books by title, author, or category.
  - Reserve or borrow books from the center.
  - View borrowing history and due dates.

### Faculty

- **Account Management**: Register, log in, view
- **Book Interaction**:
  - Request new books to be added to the collection.

### Staff

- **Book Management**:
  - Add, update, or remove books from the system.
  - Manage borrowing and reservation requests.

## Setup Instructions

### Prerequisites

Ensure you have the following installed:

- Node.js (v14 or higher)
- npm (v6 or higher)
- MongoDB

### Installation

1. **Extract the ZIP File**:
   Extract the project ZIP file to a directory of your choice.
2. **Open the Project in Visual Studio Code**:
   Open the extracted folder in Visual Studio Code.
3. **Navigate to the Backend Directory**:
   ```bash
   cd Back
   ```
4. **Install Dependencies**:
   ```bash
   npm install
   ```
5. **Start MongoDB**:
   Ensure MongoDB is running locally or remotely.
6. **Set Up Environment Variables**:
   Create a `.env` file in the `Back` folder with the following content:
   ```env
   PORT=3000
   DB_URI=mongodb://localhost:27017/bookcenter
   JWT_SECRET=your-secret-key
   ```
7. **Start the Backend Server**:
   ```bash
   npm start
   ```
   The server will be available at `http://localhost:3000`.


   API:
   Authentication Routes
Handles authentication-related routes.

POST /login
Description: Handles user login.
POST /register
Description: Handles user registration.
Book Routes
Handles book-related routes.

GET /books/
Description: Retrieves all books.
POST /books/
Description: Creates a new book.
GET /books/:id
Description: Retrieves a specific book by its ID.
PUT /books/:id
Description: Updates a specific book by its ID.
DELETE /books/:id
Description: Deletes a specific book by its ID.
POST /books/approve
Description: Approves a book.
DELETE /books/reject/:id
Description: Rejects a book by its ID.
Faculty Routes
Handles faculty-related routes.

GET /faculty/
Description: Retrieves all faculty orders.
POST /faculty/
Description: Creates a new faculty order.
Favorite Routes
Handles favorite-related routes.

GET /favorites/
Description: Retrieves all favorite books for all users.
GET /favorites/user/:userId
Description: Retrieves favorite books for a specific user.


Role Routes
Handles role-related routes.

GET /roles/
Description: Retrieves all roles.
GET /roles/:name
Description: Retrieves a specific role by its name.
Student Routes
Handles student-related routes.

GET /students/
Description: Retrieves all student orders.
GET /students/pending-approval
Description: Retrieves student orders pending approval.
User Routes
Handles user-related routes.

POST /users/register
Description: Registers a new user.
Additional routes might handle user authentication and profile management.


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

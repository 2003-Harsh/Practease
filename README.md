# Fullstack Chat Application

## Description

This is a fullstack chat application built with React (Vite) for the frontend, Node.js/Express for the backend, and MongoDB as the database. It includes features for user authentication, real-time messaging using Socket.IO, user management (admin access), and chat history download.

## Features

*   User Authentication (Login/Logout)
*   Real-time Messaging (Text and Image support)
*   Private Chats between users
*   Admin Panel for User Management (e.g., deleting chats)
*   Download Chat History as PDF (with user permissions)
*   User Online Status display
*   Responsive UI

## Technologies Used

**Frontend:**
*   React
*   Vite
*   Tailwind CSS (for styling)
*   Zustand (for state management)
*   Axios (for API calls)
*   Socket.IO Client

**Backend:**
*   Node.js
*   Express.js
*   MongoDB (Database)
*   Mongoose (ODM)
*   Socket.IO Server
*   JWT (for authentication)
*   Bcryptjs (for password hashing - common practice, assuming)
*   Cloudinary (for image uploads)
*   PDFKit (for PDF generation)

## Setup and Installation

**Prerequisites:**

*   Node.js installed
*   MongoDB instance running (local or hosted)
*   Cloudinary account (for image uploads - needed for image features)

**1. Clone the repository:**

```bash
git clone <repository_url> # Replace with your repository URL
cd fullstack-chat-app
```

**2. Backend Setup:**

Navigate to the `backend` directory:

```bash
cd backend
```

Install backend dependencies:

```bash
npm install
```

Create a `.env` file in the `backend` directory and add the following environment variables:

```env
PORT=5000 # Or your desired port
MONGO_DB_URI=<your_mongodb_connection_string>
JWT_SECRET=<your_jwt_secret_key>
CLOUDINARY_CLOUD_NAME=<your_cloudinary_cloud_name>
CLOUDINARY_API_KEY=<your_cloudinary_api_key>
CLOUDINARY_API_SECRET=<your_cloudinary_api_secret>
# Add any other environment variables your backend uses
```

Replace the placeholder values with your actual credentials and settings.

**3. Frontend Setup:**

Navigate to the `frontend` directory:

```bash
cd ../frontend
```

Install frontend dependencies:

```bash
npm install
```

Create a `.env` file in the `frontend` directory if your frontend code uses environment variables (e.g., for API base URL, Cloudinary keys if uploading directly from frontend, etc.). For example:

```env
VITE_BACKEND_URL=http://localhost:5000
# Add any other VITE_* environment variables your frontend uses
```

## Running the Application

**1. Start the Backend:**

Navigate to the `backend` directory and run:

```bash
cd ../backend
npm run dev # Or the command to start your backend (e.g., node index.js)
```

This will start the backend server, typically on the PORT specified in your `.env` file.

**2. Start the Frontend:**

Navigate to the `frontend` directory and run:

```bash
cd ../frontend
npm run dev # Or the command to start your frontend dev server
```

This will start the frontend development server, typically on port 5173.

The application should now be accessible in your browser at `http://localhost:5173` (or the port your frontend server uses).

## Folder Structure

A simplified view of the project structure:

```
fullstack-chat-app/
├── backend/
│   ├── src/
│   │   ├── controllers/
│   │   ├── middleware/
│   │   ├── models/
│   │   ├── routes/
│   │   ├── lib/ 
│   │   └── ...
│   ├── .env
│   └── package.json
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── store/ 
│   │   ├── lib/
│   │   └── ...
│   ├── public/
│   ├── index.html
│   ├── package.json
│   ├── vite.config.js
│   └── ...
├── .gitignore
├── README.md
└── ... (other root files)
```

## Credits

*   Created and Developed by Harsh Srivastav
*   An Initiative by Talent Transformation Team

---

# NexusChat Application

## Overview

Welcome to the NexusChat Application, a robust and scalable chat platform built using the MERN stack (MongoDB, Express.js, React.js, Node.js) and powered by Socket.io for real-time communication. This application enables users to engage in dynamic, real-time conversations with support for private messages, group chats, and user presence notifications.

## Features

- **Frontend:** Built with React
- **Styling:** Tailwind CSS
- **File Handling:** Multer for File and Image Storage
- **File Download:** Easy File Downloading 
- **Fun Conversations:** Emoji Support
- **Backend:** Node.js and Express
- **Database:** MongoDB for Efficient Data Storage
- **State Management:** Zustand for Seamless State Management
- **API Calls:** Axios for Smooth API Interactions
- **Code Quality:** Structured and Maintainable Code
- **Real-time Messaging:** Instant messaging between users using WebSockets with Socket.io.
- **User Authentication:** Secure user registration and login using JWT (JSON Web Tokens).
- **Group Chats:** Create and manage multiple chat rooms or channels for group discussions.
- **User Presence:** Track and display user online/offline status.
- **Profile Management:** Users can update their profile information and upload profile pictures.
- **Responsive Design:** Fully responsive UI that adapts to various screen sizes.

## Technologies Used

- **MongoDB:** NoSQL database for storing user data, chat messages, and chat room information.
- **Express.js:** Web framework for Node.js to handle API routes and server-side logic.
- **React.js:** Frontend library for building interactive user interfaces.
- **Node.js:** JavaScript runtime environment for building the backend server.
- **Tailwind CSS:** For UI Design
- **Zustand:** For State Seamless State Management
- **Multer:** For File and Image Storage 
- **Socket.io:** Real-time communication library for bidirectional event-based communication between clients and server.
- **JWT (JSON Web Tokens):** Authentication mechanism for securing API endpoints.

## Getting Started

### Prerequisites

- Node.js (v14 or higher)
- MongoDB (locally or Atlas cloud instance)
- Git

### Installation

1. **Clone the Repository:**

    ```sh
    git clone https://github.com/teja-86/NexusChat.git
    cd NexusChat
    ```

2. **Install Server Dependencies:**

    ```sh
    cd server
    npm install
    ```

3. **Install Client Dependencies:**

    ```sh
    cd ../client
    npm install
    ```

4. **Set Up Environment Variables:**

    Create a `.env` file in the `server` directory with the following content:

    ```env
    PORT=5173
    MONGO_URI=your-mongodb-connection-string
    JWT_KEY=your-jwt-secret-key
    ```

    Replace `your-mongodb-connection-string` with your MongoDB URI and `your-jwt-secret-key` with a secure secret key for JWT.

5. **Run the Application:**

    - **Start the Server:**

        ```sh
        cd server
        npm start
        ```

    - **Start the Client:**

        ```sh
        cd ../client
        npm start
        ```

    The application will be accessible at `http://localhost:8747` for the client and `http://localhost:5173` for the server.

## API Endpoints

- **POST /api/auth/signup:** Register a new user.
- **POST /api/auth/login:** Authenticate a user and generate a JWT.
- **GET /api/auth/userinfo:** Retrieve user information (requires authentication).
- **POST /api/auth/update-profile:** Update user profile information.
- **POST /api/auth/add-profile-image:** Upload a profile image.
- **DELETE /api/auth/remove-profile-image:** Remove the user's profile image.

## Running Tests

To run tests, ensure you are in the `client` or `server` directory and use:

```sh
npm test

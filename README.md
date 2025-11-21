# MPK (Majelis Perwakilan Kelas) Web Application

## Overview
This project is a web application for MPK (Majelis Perwakilan Kelas) built using React for the frontend, Node.js with Express for the backend, and MongoDB for the database. The application implements JWT authentication and provides various features for managing user information and member activities.

## Project Structure
The project is structured into two main parts: the client and the server.

### Client
- **Location:** `client/`
- **Technologies:** React, TypeScript, Tailwind CSS
- **Main Files:**
  - `public/index.html`: Entry point for the React application.
  - `src/main.tsx`: Renders the App component and sets up routing.
  - `src/App.tsx`: Main application component with routing and layout.
  - `src/pages/`: Contains various page components (Dashboard, Login, Register, Members).
  - `src/components/`: Contains reusable components (AuthForm, MemberList, Navbar).
  - `src/hooks/useAuth.ts`: Custom hook for managing authentication state.
  - `src/services/api.ts`: API call functions.
  - `src/contexts/AuthContext.tsx`: Context for global authentication state.
  - `src/styles/index.css`: Global styles including Tailwind CSS imports.

### Server
- **Location:** `server/`
- **Technologies:** Node.js, Express, MongoDB
- **Main Files:**
  - `src/app.ts`: Sets up the Express application, middleware, and routes.
  - `src/server.ts`: Entry point for the server.
  - `src/config/db.ts`: Database connection logic for MongoDB.
  - `src/controllers/`: Contains controllers for handling requests (auth and member).
  - `src/routes/`: Defines routes for authentication and member management.
  - `src/models/`: Contains MongoDB models (User and Member).
  - `src/middleware/auth.middleware.ts`: Middleware for protecting routes.
  - `src/utils/jwt.ts`: Utility functions for JWT token management.

## Features
- User authentication (login and registration).
- Dashboard for displaying statistics and aspirations.
- Member management with a list of users.
- Responsive design using Tailwind CSS.

## Getting Started
1. Clone the repository.
2. Navigate to the `client` and `server` directories and install dependencies:
   - For the client: `npm install`
   - For the server: `npm install`
3. Set up the environment variables in the `.env` file based on the `.env.example` provided.
4. Start the server:
   - Navigate to the `server` directory and run: `npm start`
5. Start the client:
   - Navigate to the `client` directory and run: `npm start`

## License
This project is licensed under the MIT License.
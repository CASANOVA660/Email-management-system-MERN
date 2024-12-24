# Email Management System

## Overview
The Email Management System is a full-stack application built using the MERN stack (MongoDB, Express.js, React, and Node.js). This system allows users to manage their email communications efficiently by providing features like composing, sending, receiving, and organizing emails in a user-friendly interface.

## Features
- **User Authentication:** Sign up, log in, and log out functionality with secure password encryption.
- **Compose Emails:** Create and send emails to other registered users.
- **Inbox and Sent Items:** View received and sent emails in organized folders.
- **Email Labels:** Tag emails with custom labels for better organization.
- **Search:** Search functionality to quickly find emails by subject or sender.
- **Responsive Design:** A fully responsive UI for optimal use on desktops, tablets, and smartphones.

## Tech Stack
### Frontend
- **React**: For building the dynamic and responsive user interface.
- **Bootstrap**: For styling and ensuring a clean, user-friendly design.

### Backend
- **Node.js**: For handling server-side logic.
- **Express.js**: For creating RESTful APIs.

### Database
- **MongoDB**: For storing user and email data.

### Additional Tools
- **Mongoose**: For MongoDB object modeling.
- **JWT (JSON Web Token)**: For secure authentication.
- **Nodemailer**: For email-sending functionality.

## Installation
### Prerequisites
Ensure you have the following installed:
- [Node.js](https://nodejs.org/)
- [MongoDB](https://www.mongodb.com/)
- npm (comes with Node.js)

### Steps to Set Up
1. **Clone the repository:**
   ```bash
   git clone https://github.com/CASANOVA660/Email-management-system-MERN.git
   cd email-management-system
   ```

2. **Install dependencies:**
   - Backend:
     ```bash
     cd server
     npm install
     ```
   - Frontend:
     ```bash
     cd ../client
     npm install
     ```

3. **Set up environment variables:**
   - Create a `.env` file in the `server` folder and add the following:
     ```env
     MONGO_URI=your-mongodb-connection-string
     JWT_SECRET=your-jwt-secret
     EMAIL_USER=your-email@example.com
     EMAIL_PASS=your-email-password
     ```

4. **Run the application:**
   - Start the backend:
     ```bash
     cd server
     npm start
     ```
   - Start the frontend:
     ```bash
     cd ../client
     npm start
     ```

5. **Access the application:**
   Open your browser and go to `http://localhost:3000`.

## Folder Structure
```
email-management-system
├── client          # React frontend
│   ├── public      # Public assets
│   └── src         # Source code
├── server          # Backend server
│   ├── controllers # API controllers
│   ├── models      # MongoDB models
│   ├── routes      # API routes
│   └── utils       # Utility functions
├── .gitignore      # Files and folders to ignore in Git
├── README.md       # Project documentation
└── package.json    # Project metadata and dependencies
```

## API Endpoints
### Authentication
- **POST** `/api/auth/register`: Register a new user.
- **POST** `/api/auth/login`: Log in a user and return a JWT.

### Emails
- **POST** `/api/emails/send`: Send an email.
- **GET** `/api/emails/inbox`: Fetch all received emails.
- **GET** `/api/emails/sent`: Fetch all sent emails.

## Contributing
Contributions are welcome! Please follow these steps:
1. Fork the repository.
2. Create a new branch for your feature or bug fix:
   ```bash
   git checkout -b feature-name
   ```
3. Commit your changes and push them:
   ```bash
   git commit -m "Add feature-name"
   git push origin feature-name
   ```
4. Open a Pull Request on GitHub.

## License
This project is licensed under the [MIT License](LICENSE).

---
Feel free to customize and expand this README as needed!


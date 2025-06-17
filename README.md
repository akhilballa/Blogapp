# Blog Application

A full-stack MERN (MongoDB, Express.js, React.js, Node.js) blog application that allows users to create, read, update, and delete blog posts. The application features user authentication, personal blog management, and a modern, responsive UI built with Material-UI.

## Features

- 🔐 User Authentication (Register/Login)
- ✍️ Create, Read, Update, and Delete Blog Posts
- 👤 User-specific Blog Management
- 🎨 Modern UI with Material-UI Components
- 📱 Responsive Design
- 🔄 Real-time State Management with Redux
- 🎯 Toast Notifications for User Feedback

## Tech Stack

### Frontend
- React.js
- Material-UI (@mui/material)
- Redux Toolkit for State Management
- React Router for Navigation
- Axios for API Requests
- React Hot Toast for Notifications

### Backend
- Node.js
- Express.js
- MongoDB with Mongoose
- bcrypt for Password Hashing
- CORS for Cross-Origin Resource Sharing
- Morgan for HTTP Request Logging

## Prerequisites

Before running this application, make sure you have the following installed:
- Node.js (v14 or higher)
- MongoDB
- npm or yarn

## Installation

1. Clone the repository:
```bash
git clone <your-repository-url>
cd blogapp
```

2. Install server dependencies:
```bash
npm install
```

3. Install client dependencies:
```bash
cd client
npm install
```

4. Create a `.env` file in the root directory and add the following:
```
PORT=8080
MONGODB_URI=your_mongodb_connection_string
DEV_MODE=development
```

## Running the Application

1. Start the development server (runs both frontend and backend):
```bash
npm run dev
```

2. Or run frontend and backend separately:
```bash
# Run backend
npm run server

# Run frontend
npm run client
```

The application will be available at:
- Frontend: http://localhost:3000
- Backend: http://localhost:8080

## API Endpoints

### User Routes
- POST `/api/v1/user/register` - Register a new user
- POST `/api/v1/user/login` - Login user
- GET `/api/v1/user/all-users` - Get all users

### Blog Routes
- GET `/api/v1/blog/all-blog` - Get all blogs
- POST `/api/v1/blog/create-blog` - Create a new blog
- PUT `/api/v1/blog/update-blog/:id` - Update a blog
- GET `/api/v1/blog/get-blog/:id` - Get a specific blog
- DELETE `/api/v1/blog/delete-blog/:id` - Delete a blog
- GET `/api/v1/blog/user-blog/:id` - Get user's blogs

## Project Structure

```
blogapp/
├── client/                 # Frontend React application
│   ├── src/
│   │   ├── components/    # Reusable components
│   │   ├── pages/        # Page components
│   │   ├── redux/        # Redux store and slices
│   │   └── App.js        # Main App component
├── controllers/           # Route controllers
├── models/               # Mongoose models
├── routes/              # Express routes
├── config/              # Configuration files
└── server.js           # Entry point
```

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the ISC License.

## Author

Akhil

## Acknowledgments

- Material-UI for the component library
- React community for the amazing tools and libraries

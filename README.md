# KaalaSetu 🚀

A modern AI-powered content generation platform that allows users to create videos, audio, and graphics through an intuitive chat interface. Built with React frontend and Node.js backend, featuring user authentication and session management.

## ✨ Features

- **Multi-Modal Content Generation**: Generate videos, audio, and graphics from text prompts
- **Chat-Based Interface**: Intuitive conversation-style interface for content creation
- **Session Management**: Save and manage multiple conversation sessions
- **User Authentication**: Secure login/signup system with JWT tokens
- **Real-time Chat**: Interactive chat experience with message history
- **Responsive Design**: Modern UI built with Tailwind CSS and dark theme support
- **Session Persistence**: Automatically save and restore conversation history

## 🛠️ Tech Stack

### Frontend
- **React 18** - Modern React with hooks and functional components
- **React Router DOM** - Client-side routing
- **Tailwind CSS** - Utility-first CSS framework
- **React Toastify** - Toast notifications
- **Local Storage** - Client-side data persistence

### Backend
- **Node.js** - JavaScript runtime
- **Express.js** - Web application framework
- **MongoDB** - NoSQL database with Mongoose ODM
- **JWT** - JSON Web Tokens for authentication
- **bcrypt** - Password hashing
- **Joi** - Data validation
- **CORS** - Cross-origin resource sharing

## 📁 Project Structure

```
kaalasetu/
├── backend/                 # Node.js/Express backend
│   ├── Controllers/        # Request handlers
│   ├── Middlewares/        # Authentication & validation
│   ├── Models/            # MongoDB schemas
│   ├── Routes/            # API route definitions
│   └── index.js           # Server entry point
├── frontend/              # React frontend
│   ├── public/           # Static assets
│   ├── src/
│   │   ├── components/   # Reusable UI components
│   │   ├── pages/        # Page components
│   │   └── App.js        # Main app component
│   └── package.json
└── README.md
```

## 🚀 Getting Started

### Prerequisites

- Node.js (v14 or higher)
- MongoDB (local installation or MongoDB Atlas)
- npm or yarn package manager

### Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd kaalasetu
   ```

2. **Backend Setup**
   ```bash
   cd backend
   npm install
   ```

3. **Frontend Setup**
   ```bash
   cd ../frontend
   npm install
   ```

4. **Environment Configuration**

   Create a `.env` file in the backend directory:
   ```env
   PORT=4000
   MONGODB_URI=mongodb://localhost:27017/kaalasetu
   JWT_SECRET=your_jwt_secret_here
   ```

5. **Start the Development Servers**

   **Backend (Terminal 1):**
   ```bash
   cd backend
   npm start
   ```
   Server will run on `http://localhost:4000`

   **Frontend (Terminal 2):**
   ```bash
   cd frontend
   npm start
   ```
   App will run on `http://localhost:3000`

## 📖 Usage

### Authentication
1. Navigate to the application
2. Create a new account or login with existing credentials
3. JWT tokens are automatically managed for session persistence

### Content Generation
1. **Start a New Chat**: Click "New Chat" to begin a fresh conversation
2. **Select Content Type**: Choose between Video, Audio, or Graphics generation
3. **Enter Your Prompt**: Describe what you want to create
4. **Generate Content**: Submit your prompt to generate content
5. **Manage Sessions**: Access previous conversations from the sidebar

### Session Management
- **Create Sessions**: Each new chat creates a session automatically
- **Load Sessions**: Click on previous sessions to restore conversation history
- **Delete Sessions**: Remove unwanted sessions (feature can be extended)

## 🔧 API Endpoints

### Authentication
- `POST /auth/signup` - User registration
- `POST /auth/login` - User login

### Sessions
- `GET /api/sessions` - Get user sessions
- `GET /api/sessions/:id/messages` - Get session messages
- `POST /api/sessions` - Create new session

### Content Generation
- `POST /api/generate/video` - Generate video content
- `POST /api/generate/audio` - Generate audio content
- `POST /api/generate/graphics` - Generate graphics content

## 🎨 UI Components

- **Sidebar**: Session management and navigation
- **Chat Interface**: Main conversation area with message history
- **Prompt Input**: Multi-type content generation interface
- **Output Viewer**: Display generated content (extensible)
- **User Menu**: Profile and logout functionality

## 🔒 Security Features

- **JWT Authentication**: Secure token-based authentication
- **Password Hashing**: bcrypt for secure password storage
- **Input Validation**: Joi schema validation for all inputs
- **CORS Protection**: Configured for secure cross-origin requests
- **Protected Routes**: Authentication middleware for sensitive endpoints

## 🚀 Deployment

### Backend (Vercel)
The backend includes `vercel.json` configuration for easy deployment on Vercel.

### Frontend (Vercel)
The frontend includes `vercel.json` configuration for deployment on Vercel.

### Environment Variables
Ensure all environment variables are properly configured in your deployment platform.

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the ISC License.

## 🆘 Support

For support and questions:
- Create an issue in the repository
- Contact the development team

## 🔮 Future Enhancements

- [ ] Real AI integration for content generation
- [ ] File upload capabilities
- [ ] Advanced content editing tools
- [ ] Collaboration features
- [ ] Analytics dashboard
- [ ] Mobile app development

---

**KaalaSetu** - Bridging creativity with AI technology 🎨✨# kaalasetu

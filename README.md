# Autonomous LLM Agents

## Capstone Project - Autonomous LLM Agents for Multi-Step Tasks

This is a capstone project that demonstrates the implementation of autonomous Large Language Model (LLM) agents capable of handling complex, multi-step tasks. The system integrates authentication, DevOps workflows, and travel planning functionalities, showcasing how AI agents can autonomously execute and coordinate various processes.

### Features

- **Authentication System**: Secure user registration and login with JWT tokens
- **Travel Planning Agents**: Multi-agent system for trip planning, requirements analysis, execution, and review
- **DevOps Integration**: Jenkins pipeline for CI/CD automation
- **Containerized Deployment**: Docker Compose setup for easy deployment

### Tech Stack

#### Backend
- **Node.js** with Express.js framework
- **MongoDB** for data persistence
- **JWT** for authentication
- **Docker** for containerization

#### Frontend
- **React** with Vite build tool
- **CSS** for styling
- **Context API** for state management

#### AI/ML
- **Python** for LLM integration and AI tutoring
- **Custom LLM utilities** for agent communication

#### DevOps
- **Jenkins** for CI/CD pipelines
- **Docker Compose** for multi-container orchestration

### Prerequisites

Before running this project, make sure you have the following installed:

- **Node.js** (v16 or higher)
- **npm** or **yarn**
- **Python** (v3.8 or higher)
- **MongoDB** (local or cloud instance)
- **Docker** and **Docker Compose** (for containerized deployment)

### Installation and Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com/soumithgajula01/autonomous-llm-agents.git
   cd autonomous-llm-agents
   ```

2. **Install backend dependencies:**
   ```bash
   cd backend
   npm install
   ```

3. **Install frontend dependencies:**
   ```bash
   cd ../frontend
   npm install
   ```

4. **Install server dependencies (if separate):**
   ```bash
   cd ../server
   npm install
   ```

5. **Set up environment variables:**
   Create `.env` files in the backend and server directories with necessary configurations (database URL, JWT secret, etc.)

6. **Start MongoDB:**
   Ensure MongoDB is running locally or update connection strings for cloud instance.

### Running the Project

#### Option 1: Using Docker Compose (Recommended)

1. **Build and start all services:**
   ```bash
   docker-compose up --build
   ```

2. **Access the application:**
   - Frontend: http://localhost:3000
   - Backend API: http://localhost:5000
   - Additional services as configured

#### Option 2: Manual Setup

1. **Start the backend server:**
   ```bash
   cd backend
   npm start
   ```

2. **Start the frontend:**
   ```bash
   cd frontend
   npm run dev
   ```

3. **Run the Python AI script (if needed):**
   ```bash
   python ai_jee_tutor.py
   ```

4. **Start additional server (if applicable):**
   ```bash
   cd server
   npm start
   ```

### Project Structure

```
autonomous-llm-agents/
├── backend/                 # Main backend application
│   ├── controllers/         # Route controllers
│   ├── middleware/          # Authentication middleware
│   ├── models/              # MongoDB models
│   ├── routes/              # API routes
│   ├── services/            # Business logic services
│   ├── tasks/travel/        # Travel planning agents
│   └── utils/               # Utility functions
├── frontend/                # React frontend application
│   ├── src/
│   │   ├── components/      # React components
│   │   ├── context/         # React context for state
│   │   └── assets/          # Static assets
│   └── public/              # Public files
├── server/                  # Additional server (if needed)
├── ai_jee_tutor.py          # Python AI tutoring script
├── docker-compose.yml       # Docker orchestration
├── jenkinsfile              # Jenkins CI/CD pipeline
└── README.md                # Project documentation
```

### API Endpoints

- `POST /api/auth/register` - User registration
- `POST /api/auth/login` - User login
- `GET /api/tasks` - Get user tasks
- Additional endpoints for travel planning and agent interactions

### Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request


### Acknowledgments

- Capstone project demonstrating autonomous AI agent systems
- Integrates multiple technologies for full-stack development
- Showcases multi-agent coordination for complex tasks

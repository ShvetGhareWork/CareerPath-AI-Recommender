# CareerPath-AI 🎯

<div align="center">

![CareerPath-AI Banner](https://via.placeholder.com/1200x300/4F46E5/FFFFFF?text=CareerPath-AI+%7C+AI-Powered+Career+Guidance)

**An intelligent career recommendation system powered by AI to help students discover their ideal career path**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Node.js](https://img.shields.io/badge/Node.js-16+-green.svg)](https://nodejs.org/)
[![React](https://img.shields.io/badge/React-18+-blue.svg)](https://reactjs.org/)
[![MongoDB](https://img.shields.io/badge/MongoDB-5.0+-green.svg)](https://www.mongodb.com/)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com)

[Live Demo](#) • [Documentation](./DEPLOYMENT_GUIDE.md) • [Report Bug](#) • [Request Feature](#)

</div>

---

## 📖 About The Project

CareerPath-AI is an AI-powered career recommendation system designed to revolutionize how students make career decisions. Unlike traditional career counseling methods that provide generic advice, CareerPath-AI analyzes individual skills, academic performance, and personal interests to deliver **personalized, data-driven career recommendations**.

The system goes beyond simple suggestions—it performs **skill gap analysis** and recommends relevant courses, certifications, and learning resources to help students bridge the gap between their current abilities and their dream careers.

### 🎯 Why CareerPath-AI?

- **Personalized Recommendations**: Tailored career paths based on your unique profile
- **AI-Powered Analysis**: Machine learning algorithms analyze your strengths and interests
- **Skill Gap Identification**: Discover what skills you need to develop
- **Resource Suggestions**: Get curated courses and certifications
- **Interactive Chatbot**: Ask career-related questions anytime
- **Industry-Aligned**: Recommendations reflect current job market demands

---

## ✨ Features

### 🔐 **User Authentication**
- Email/password registration and login
- Google OAuth integration for quick sign-up
- Secure JWT-based authentication
- Password recovery functionality

### 👤 **Profile Management**
- Comprehensive profile creation
- Academic performance tracking
- Skills inventory (technical & soft skills)
- Interest and preference mapping

### 🤖 **AI-Powered Recommendations**
- Hybrid recommendation engine (content-based + collaborative filtering)
- Natural Language Processing for text analysis
- Real-time career path suggestions
- Personalized to individual strengths

### 📊 **Skill Gap Analysis**
- Identifies missing skills for target careers
- Provides actionable development roadmap
- Tracks skill acquisition progress

### 📚 **Learning Resources**
- Curated online courses
- Industry certifications
- Learning pathways
- Integration with course providers

### 💬 **AI Chatbot**
- Context-aware career guidance
- Answers career-related queries
- Personalized advice based on user profile

### 📈 **Career Insights**
- Job market trends
- Salary expectations
- Growth opportunities
- Industry demand analysis

---

## 🖼️ Screenshots

<div align="center">

### Home Page
<img width="1919" height="914" alt="homepage" src="https://github.com/user-attachments/assets/c5eff57d-d7b1-492a-97ef-60079b9753a8" />

*Clean, modern landing page with clear call-to-action*

### Dashboard
<img width="1919" height="907" alt="dashboard" src="https://github.com/user-attachments/assets/b12f3356-40bd-47a3-8a26-c95abc27d916" />

*Personalized dashboard with career recommendations and insights*

### Career Recommendations
<img width="1919" height="912" alt="recommendations" src="https://github.com/user-attachments/assets/4410a342-6b71-4c8f-a4db-e22f93a07c61" />

*AI-generated career suggestions with skill gap analysis*

### Chatbot Interface
<img width="560" height="878" alt="chatbot" src="https://github.com/user-attachments/assets/dd3aaa64-7eb1-42f2-b8fc-bd04d5cd72b7" />

*Interactive AI assistant for career guidance*

</div>

---

## 🛠️ Tech Stack

### **Frontend**
- **Framework**: React.js 18+
- **Styling**: CSS3, Tailwind CSS (optional)
- **State Management**: React Context API / Redux
- **HTTP Client**: Axios
- **Routing**: React Router v6

### **Backend**
- **Runtime**: Node.js 16+
- **Framework**: Express.js
- **Authentication**: JWT, Passport.js (Google OAuth)
- **API Architecture**: RESTful APIs

### **Database**
- **Primary Database**: MongoDB (NoSQL)
- **ODM**: Mongoose
- **Cloud Database**: MongoDB Atlas

### **AI/ML**
- **Language**: Python 3.8+
- **Libraries**: 
  - Scikit-learn (ML algorithms)
  - TensorFlow (Deep learning)
  - NLTK (Natural Language Processing)
  - Pandas & NumPy (Data processing)
- **AI Service**: Google Gemini API

### **External APIs**
- Job listings API (LinkedIn, Indeed)
- Course providers API (Coursera, Udemy)
- Google OAuth 2.0

### **DevOps & Tools**
- **Version Control**: Git & GitHub
- **Containerization**: Docker
- **API Testing**: Postman
- **Code Editor**: VS Code
- **Deployment**: Vercel, Render, Railway

---

## 🚀 Getting Started

Follow these steps to set up CareerPath-AI locally.

### Prerequisites

Ensure you have the following installed:

- **Node.js** (v16 or higher) - [Download](https://nodejs.org/)
- **npm** or **yarn** - Comes with Node.js
- **MongoDB** - [Download](https://www.mongodb.com/try/download/community) or use [MongoDB Atlas](https://www.mongodb.com/cloud/atlas)
- **Python** (v3.8+) - [Download](https://www.python.org/downloads/)
- **Git** - [Download](https://git-scm.com/)

### Installation

1. **Clone the repository**

```bash
git clone https://github.com/yourusername/careerpath-ai.git
cd careerpath-ai
```

2. **Install backend dependencies**

```bash
cd backend
npm install
pip install -r requirements.txt
```

3. **Install frontend dependencies**

```bash
cd ../frontend
npm install
```

4. **Set up environment variables**

Create `.env` files in both `backend` and `frontend` directories.

**Backend `.env`:**

```env
PORT=5000
NODE_ENV=development
MONGODB_URI=mongodb://localhost:27017/careerpath
JWT_SECRET=your_jwt_secret_key_here
JWT_EXPIRE=7d
GOOGLE_CLIENT_ID=your_google_client_id
GOOGLE_CLIENT_SECRET=your_google_client_secret
GOOGLE_CALLBACK_URL=http://localhost:5000/auth/google/callback
GEMINI_API_KEY=your_gemini_api_key
FRONTEND_URL=http://localhost:3000
```

**Frontend `.env`:**

```env
REACT_APP_API_URL=http://localhost:5000/api
REACT_APP_BACKEND_URL=http://localhost:5000
REACT_APP_GOOGLE_CLIENT_ID=your_google_client_id
REACT_APP_ENV=development
```

5. **Start MongoDB**

```bash
# If using local MongoDB
sudo systemctl start mongodb

# Or use MongoDB Atlas connection string in .env
```

6. **Run the application**

**Backend:**
```bash
cd backend
npm run dev
```

**Frontend:**
```bash
cd frontend
npm start
```

7. **Access the application**

- Frontend: [http://localhost:3000](http://localhost:3000)
- Backend API: [http://localhost:5000](http://localhost:5000)

---

## 🔑 Environment Variables

### Backend Variables

| Variable | Description | Required |
|----------|-------------|----------|
| `PORT` | Backend server port | Yes |
| `NODE_ENV` | Environment (development/production) | Yes |
| `MONGODB_URI` | MongoDB connection string | Yes |
| `JWT_SECRET` | Secret key for JWT tokens | Yes |
| `JWT_EXPIRE` | Token expiration time | Yes |
| `GOOGLE_CLIENT_ID` | Google OAuth client ID | Yes |
| `GOOGLE_CLIENT_SECRET` | Google OAuth secret | Yes |
| `GOOGLE_CALLBACK_URL` | OAuth callback URL | Yes |
| `GEMINI_API_KEY` | Google Gemini API key | Yes |
| `JOB_API_KEY` | Job listings API key | Optional |
| `COURSE_API_KEY` | Course provider API key | Optional |
| `FRONTEND_URL` | Frontend URL for CORS | Yes |

### Frontend Variables

| Variable | Description | Required |
|----------|-------------|----------|
| `REACT_APP_API_URL` | Backend API base URL | Yes |
| `REACT_APP_BACKEND_URL` | Backend base URL | Yes |
| `REACT_APP_GOOGLE_CLIENT_ID` | Google OAuth client ID | Yes |
| `REACT_APP_ENV` | Environment | Yes |

### How to Get API Keys

- **Google OAuth**: [Google Cloud Console](https://console.cloud.google.com/)
- **Gemini API**: [Google AI Studio](https://makersuite.google.com/app/apikey)

---

## 🏃 How to Run Locally

### Quick Start

```bash
# Clone repository
git clone https://github.com/yourusername/careerpath-ai.git
cd careerpath-ai

# Install all dependencies
npm run install:all

# Set up environment variables (see above)

# Start both frontend and backend
npm run dev
```

### Individual Services

```bash
# Backend only
cd backend
npm run dev

# Frontend only
cd frontend
npm start

# Run tests
npm test
```

---

## 🌐 Deployment

For detailed deployment instructions, see [DEPLOYMENT_GUIDE.md](./DEPLOYMENT_GUIDE.md)

### Quick Deployment Options

#### **Frontend (Vercel)**

```bash
npm install -g vercel
cd frontend
vercel
```

#### **Backend (Render)**

1. Push code to GitHub
2. Connect repository to [Render](https://render.com)
3. Add environment variables
4. Deploy

#### **Full Stack (Railway)**

1. Visit [Railway.app](https://railway.app)
2. Connect GitHub repository
3. Configure environment variables
4. Deploy automatically

---

## 📁 Folder Structure

```
careerpath-ai/
├── backend/
│   ├── config/           # Configuration files
│   ├── controllers/      # Route controllers
│   ├── models/           # Database models
│   ├── routes/           # API routes
│   ├── middleware/       # Custom middleware
│   ├── services/         # Business logic
│   │   ├── ai/          # AI/ML services
│   │   └── chatbot/     # Chatbot logic
│   ├── utils/           # Utility functions
│   ├── data/            # Seed data
│   ├── requirements.txt # Python dependencies
│   ├── package.json     # Node dependencies
│   └── server.js        # Entry point
│
├── frontend/
│   ├── public/          # Static files
│   ├── src/
│   │   ├── components/  # React components
│   │   ├── pages/       # Page components
│   │   ├── context/     # Context providers
│   │   ├── services/    # API services
│   │   ├── utils/       # Utility functions
│   │   ├── styles/      # CSS files
│   │   ├── App.js       # Main component
│   │   └── index.js     # Entry point
│   └── package.json     # Dependencies
│
├── screenshots/         # Application screenshots
├── docs/               # Documentation
├── .gitignore
├── README.md
├── DEPLOYMENT_GUIDE.md
└── LICENSE
```

---

## 🔌 API Endpoints

### Authentication

| Method | Endpoint | Description | Auth Required |
|--------|----------|-------------|---------------|
| POST | `/api/auth/register` | Register new user | No |
| POST | `/api/auth/login` | User login | No |
| GET | `/auth/google` | Google OAuth login | No |
| GET | `/auth/google/callback` | OAuth callback | No |
| POST | `/api/auth/forgot-password` | Password recovery | No |

### User Profile

| Method | Endpoint | Description | Auth Required |
|--------|----------|-------------|---------------|
| GET | `/api/user/profile` | Get user profile | Yes |
| PUT | `/api/user/profile` | Update profile | Yes |
| POST | `/api/user/skills` | Add skills | Yes |
| DELETE | `/api/user/skills/:id` | Remove skill | Yes |

### Career Recommendations

| Method | Endpoint | Description | Auth Required |
|--------|----------|-------------|---------------|
| POST | `/api/recommendations` | Get career recommendations | Yes |
| GET | `/api/recommendations/history` | View past recommendations | Yes |
| GET | `/api/careers` | List all careers | No |
| GET | `/api/careers/:id` | Get career details | No |

### Courses & Resources

| Method | Endpoint | Description | Auth Required |
|--------|----------|-------------|---------------|
| GET | `/api/courses` | Get course recommendations | Yes |
| GET | `/api/courses/:id` | Get course details | No |
| POST | `/api/courses/save` | Save course to profile | Yes |

### Chatbot

| Method | Endpoint | Description | Auth Required |
|--------|----------|-------------|---------------|
| POST | `/api/chatbot/query` | Ask career question | Yes |
| GET | `/api/chatbot/history` | Get chat history | Yes |

### Admin (if applicable)

| Method | Endpoint | Description | Auth Required |
|--------|----------|-------------|---------------|
| POST | `/api/admin/careers` | Add new career | Yes (Admin) |
| PUT | `/api/admin/careers/:id` | Update career | Yes (Admin) |
| DELETE | `/api/admin/careers/:id` | Delete career | Yes (Admin) |

---

## 🤝 Contributing

We welcome contributions from the community! Here's how you can help:

### How to Contribute

1. **Fork the repository**

```bash
git clone https://github.com/yourusername/careerpath-ai.git
```

2. **Create a feature branch**

```bash
git checkout -b feature/AmazingFeature
```

3. **Make your changes**

4. **Commit your changes**

```bash
git commit -m 'Add some AmazingFeature'
```

5. **Push to the branch**

```bash
git push origin feature/AmazingFeature
```

6. **Open a Pull Request**

### Contribution Guidelines

- Follow the existing code style
- Write clear commit messages
- Add tests for new features
- Update documentation as needed
- Ensure all tests pass before submitting PR

### Code of Conduct

Please be respectful and constructive in all interactions. We're here to learn and build together!

---

## 📄 License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

```
MIT License

Copyright (c) 2025 CareerPath-AI Team

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
```

---

## 👥 Team

**CareerPath-AI** is developed by students from Universal College of Engineering, Mumbai:

- **Prathamesh Jaiswar** - [GitHub](#) | [LinkedIn](#)
- **Shvet Ghare** - [GitHub](#) | [LinkedIn](#)
- **Naitik Butani** - [GitHub](#) | [LinkedIn](#)
- **Shreya Gharat** - [GitHub](#) | [LinkedIn](#)

**Project Guide:** Mr. Anurag Singh

---

## 📞 Contact

Have questions or suggestions? Reach out to us!

- **Email**: careerpathai@example.com
- **GitHub Issues**: [Create an issue](https://github.com/yourusername/careerpath-ai/issues)
- **LinkedIn**: [Project Page](#)

---

## 🙏 Acknowledgments

We would like to thank:

- **Universal College of Engineering** for providing resources and support
- **Mr. Anurag Singh** for guidance throughout the project
- **Google** for Gemini API access
- **MongoDB** for database solutions
- **Open-source community** for amazing tools and libraries

---

## 📊 Project Status

- ✅ **Phase 1**: Core recommendation engine - Complete
- ✅ **Phase 2**: User authentication & profiles - Complete
- ✅ **Phase 3**: AI chatbot integration - Complete
- 🔄 **Phase 4**: Mobile application - In Progress
- 📅 **Phase 5**: Real-time job market integration - Planned

---

## 🌟 Star History

If you find this project helpful, please consider giving it a ⭐!

[![Star History Chart](https://api.star-history.com/svg?repos=yourusername/careerpath-ai&type=Date)](https://star-history.com/#yourusername/careerpath-ai&Date)

---

<div align="center">

**Made with ❤️ by the CareerPath-AI Team**

[⬆ Back to Top](#careerpath-ai-)

</div>


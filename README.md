<div align="center">
  <h1>⚖️ AdvocAI: AI-Powered Legal Document Navigator</h1>
  <p><strong>Intelligent Legal Tech for Document Analysis, Drafting, and Lawyer Collaboration</strong></p>

  [![React](https://img.shields.io/badge/React-19-blue.svg)](https://reactjs.org/)
  [![Vite](https://img.shields.io/badge/Vite-7-purple.svg)](https://vitejs.dev/)
  [![Django](https://img.shields.io/badge/Django-5.2-green.svg)](https://www.djangoproject.com/)
  [![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)](https://www.python.org/)
  [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
</div>

<br />

## 📖 Overview

**AdvocAI** is a comprehensive, full-stack application designed to bridge the gap between complex legal jargons and everyday understanding. By leveraging the power of advanced Generative AI models, AdvocAI provides users with an intelligent toolset for analyzing contracts, drafting accurate legal documents, and securely connecting with certified legal professionals. 

Whether you are a freelancer needing an NDA or a startup wanting to analyze terms of service, AdvocAI empowers you to make informed legal decisions with confidence and clarity.

## ✨ Key Features

- **🧠 AI Document Analyzer**: Automatically parses uploaded legal texts to detect risks, extract key clauses, and generate plain-English summaries.
- **📝 Smart Legal Drafter**: Uses AI to generate standardized legal documents based on custom user inputs and requirements.
- **🤝 Lawyer Connect Marketplace**: A dedicated portal allowing clients to find and connect with vetted legal professionals based on specialization.
- **💬 Real-Time Collaboration**: Integrated chat interface for seamless communication and document sharing between lawyers and clients.
- **✍️ Secure E-Signatures**: Built-in support for document signing and version control.
- **🎨 Modern & Responsive UI**: A highly polished, accessible interface utilizing Radix UI, Tailwind CSS, and subtle 3D particle backgrounds for a premium user experience.

## 🛠️ Technology Stack

### Frontend Architecture
- **Framework:** React 19, React Router 7, Vite
- **Styling:** Tailwind CSS, tailwind-merge, tailwindcss-animate
- **UI Components:** Radix UI primitives, Lucide Icons
- **Visuals & 3D:** `@react-three/fiber`, `@react-three/drei`, `tsparticles`
- **Networking & State:** Axios (with custom auth interceptors), React Context API

### Backend Architecture
- **Framework:** Django 5, Django REST Framework
- **Authentication:** JWT (JSON Web Tokens) via SimpleJWT
- **AI Integration:** Langchain, Google Generative AI (Gemini), OpenAI
- **Databases:** SQLite (Relational structure), MongoDB (Document & Comment storage)
- **Task Queues:** Celery & Redis (for asynchronous background jobs)
- **PDF Generation:** xhtml2pdf, PyMuPDF, ReportLab

## 🚀 Getting Started

Follow these steps to set up the project locally for development.

### Prerequisites
- **Node.js** (v18 or higher) & **npm**
- **Python** (v3.10 or higher)
- **Redis** server (for Celery workers)
- API Keys for Google Gemini / OpenAI (depending on active integrations)

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/AdvocAI_SE_Project.git
cd AdvocAI_SE_Project
```

### 2. Frontend Setup
```bash
cd frontend
npm install
# Create a .env file and add your VITE_API_BASE_URL (defaults to http://localhost:8000/)
npm run dev
```
The frontend will start on `http://localhost:5173`.

### 3. Backend Setup
```bash
cd backend
python -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts\activate
pip install -r requirement.txt

# Create a .env file in the backend directory for your database and AI API keys
python manage.py migrate
python manage.py runserver
```
The backend API will run on `http://localhost:8000`.

## 📂 Project Structure

- `/frontend/` - Contains the React + Vite application. Follows a feature-based folder structure with reusable components and contexts.
- `/backend/` - Contains the Django server. Modularized into apps such as `authentication`, `document_summarizer`, `legal_doc_generator`, and `ai_generator`.
- `/32/` - Contains complete software engineering documentations, UML diagrams (Use Case, Sequence, Class), system architectures, and final project reports.

## 🤝 Contributing

We welcome contributions to make AdvocAI even better! 
1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.

---
<div align="center">
  <i>Built with ❤️ by Group 32</i>
</div>

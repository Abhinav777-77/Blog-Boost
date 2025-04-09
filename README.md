# 🚀 Blog Boost — AI-Powered Content Creation Tool

**Blog Boost** is a full-stack AI-powered platform designed to help writers and bloggers effortlessly generate high-quality blog content and visuals. It leverages LLaMA 3 for intelligent text generation and Flux API for stunning AI-generated images — all wrapped in a modern MERN stack application.

---

## 🛠️ Tech Stack

### Frontend
- React.js
- React Router
- CSS Modules

### Backend
- Node.js + Express.js (API server)
- Flask (Python microservice for LLaMA 3 model)

### AI & ML
- LLaMA 3 via Flask (for blog content generation)
- Flux Image API (for AI-generated blog images)

### Database
- MongoDB (cloud or local)

---

## 📁 Folder Structure

blog-boost/ │ ├── backend/ │ ├── server.js # Express server │ ├── app.py # Flask server for LLaMA 3 │ ├── package.json │ └── ... │ ├── frontend/ │ ├── public/ │ │ ├── index.html │ │ └── ... │ ├── src/ │ │ ├── pages/ │ │ │ ├── Loginpage/ │ │ │ ├── Mypost/ │ │ │ ├── TitlePage/ │ │ │ ├── generatorpage/ │ │ │ ├── news/ │ │ │ └── ... │ │ ├── App.js │ │ └── index.js │ ├── package.json │ └── ... │ └── README.md

yaml
Copy
Edit

---

## ✨ Features

- 🧠 AI-generated blog titles and full-length content using LLaMA 3
- 🖼️ AI-generated blog visuals using the Flux API
- 🔐 User login and authentication system
- 📝 My Posts: Save, view, and manage your generated blogs
- 📰 Trending news snippets for content inspiration
- 🎲 Random blog idea generator for creative boosts

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/yourusername/blog-boost.git
cd blog-boost
2. Set up the Flask server (LLaMA 3)
bash
Copy
Edit
cd backend
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
python app.py
Runs Flask server on http://localhost:5001 to serve LLaMA 3 text generation.

3. Start the Node.js backend
bash
Copy
Edit
cd backend
npm install
node server.js
Runs Express backend on http://localhost:5000

4. Run the React frontend
bash
Copy
Edit
cd frontend
npm install
npm start
React app runs on http://localhost:3000

🌐 Environment Variables
Backend .env
env
Copy
Edit
LLAMA_API_URL=http://localhost:5001/generate
FLUX_API_KEY=your_flux_api_key
MONGO_URI=your_mongodb_connection_string
Frontend .env
env
Copy
Edit
REACT_APP_BACKEND_URL=http://localhost:5000
REACT_APP_LLAMA_API_URL=http://localhost:5001/generate
📡 API Overview
🔤 Text Generation (LLaMA 3 via Flask)
POST /generate
Request:

json
Copy
Edit
{
  "prompt": "Write a blog post about the future of AI"
}
🖼️ Image Generation (Flux API)
POST /generate-image
Request:

json
Copy
Edit
{
  "description": "AI transforming the world"
}


## 🪪 License

This project is licensed under the **MIT License**.  
See the [LICENSE](./LICENSE) file for more information.

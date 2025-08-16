AI Chatbot Using Django & React

A modern AI-powered chatbot web app built with Django (backend) and React (frontend), leveraging OpenAI’s API to deliver dynamic, natural language responses.

Table of Contents

Features

Tech Stack

Prerequisites

Installation

Usage

Project Structure

Contributing

License

Features

Full-stack app with Django for backend and React for frontend.

Communicates with OpenAI's API for generating intelligent chatbot responses.

Supports asynchronous conversation via a sleek chat interface.

Easily extensible for embedding in larger applications.

Tech Stack

Backend: Django

Frontend: React.js

AI Service: OpenAI API

Other Tools: Axios (HTTP requests), Dotenv for environment configuration

Prerequisites

Make sure you have installed:

Python (3.8+)

Node.js & npm (or yarn)

An OpenAI API key

pipenv or venv for virtual environment (optional)

Installation
Backend Setup
# Navigate to the backend directory
cd backend

# Create and activate virtual environment
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate

# Install dependencies
pip install django djangorestframework python-dotenv openai

# Create .env file with your OpenAI API key
echo "OPENAI_API_KEY=your_api_key_here" > .env

# Run migrations and start the server
python manage.py migrate
python manage.py runserver

Frontend Setup
# Open a new terminal and go to the frontend directory
cd frontend

# Install dependencies
npm install

# Start React development server
npm start

Usage

Open http://localhost:3000 in your browser.

Type your message and hit Enter or click Send.

The chatbot responds using OpenAI’s API via Django backend.

Project Structure
project-root/
├── backend/
│   ├── chatbot_app/
│   │   ├── views.py         # API logic interacting with OpenAI
│   │   └── urls.py
│   ├── manage.py
│   └── ...
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   └── App.js           # React app with chat UI
│   └── package.json
├── README.md
└── .env.example              # Template for environment variables

Contributing

Contributions, suggestions, and feature requests are welcome! Feel free to open issues or submit pull requests to help improve this project.

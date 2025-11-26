# 🌟 Gemini AI Chatbot

A simple **Flask-based AI chatbot** using **Google Gemini API** for generating intelligent responses.  
This project allows users to chat with AI directly through a web interface.

---

## 🗂️ Project Structure

AI_Chatbot/
│
├── app.py                 # Main Flask app
├── requirements.txt       # Python dependencies
├── .env                   # Environment variables (API Key)
│
├── templates/
│   └── index.html         # Frontend HTML
│
└── static/
    ├── css/style.css      # Stylesheet
    └── js/script.js       # JavaScript for frontend

---

## ⚡ Setup Instructions

### 1️⃣ Create Virtual Environment

#### Linux / Mac
```bash
python3 -m venv venv
source venv/bin/activate
```

#### Windows
```bash
python -m venv venv
venv\Scripts\activate
```

---

### 2️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

> **Note:** Make sure `requirements.txt` contains:
Flask
requests
python-dotenv

---

### 3️⃣ Get Gemini API Key

1. Open [Google AI Studio](https://aistudio.google.com/apikey)  
2. Sign in with your **Gmail account**  
3. Click **“Create API Key”** → choose **New Project**  
4. Copy the **API key**

> **Important:** This key is required for the chatbot to work. Without it, the app will show:  
> `RuntimeError: Missing GEMINI_API_KEY in .env`

---

### 4️⃣ Add API Key to `.env`

Create a file called `.env` in your project root:

```text
GEMINI_API_KEY=YOUR_API_KEY_HERE
```

> Replace `YOUR_API_KEY_HERE` with the API key you just generated.

---

### 5️⃣ Run the Flask App

```bash
python app.py

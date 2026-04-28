# JudgeMe

**"Same crime. Different face. Different fate."**

A web app that exposes bias in AI sentencing tools by simulating how identical crimes receive wildly different risk scores based on defendant demographics. This is a demonstration built for the Google Solution Challenge 2026.

## Tech Stack
- Frontend: React, Vite, Tailwind CSS
- Tech stack: React, Vite, Tailwind, FastAPI, Python, Gemini 2.5 Flash, Firebase Firestore, Google Cloud Runre
- Deployment: Docker / Google Cloud Run

## Setup Instructions

1. **Clone repo**
   ```bash
   git clone <repository-url>
   cd judgeme
   ```

2. **Backend Setup**
   ```bash
   cd backend
   pip install -r requirements.txt
   ```
   Add `GEMINI_API_KEY` to `backend/.env` (use `backend/.env.example` as a template).
   Optionally, add `FIREBASE_CREDENTIALS_PATH` if you want to store history.
   ```bash
   uvicorn main:app --reload
   ```

3. **Frontend Setup**
   Open a new terminal:
   ```bash
   cd judgeme/frontend
   npm install
   npm run dev
   ```

4. Open your browser to `http://localhost:5173`.

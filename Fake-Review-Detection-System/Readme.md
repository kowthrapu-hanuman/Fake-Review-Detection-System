# Fake Review Detection System

This repository contains a complete fake review detection app with a **FastAPI backend** and **React frontend**.

## Project overview

- **Backend**: Fake-Review-Detection-System/backend
- **Frontend**: Fake-Review-Detection-System/frontend
- **Goal**: Identify fake product reviews and provide confidence, risk level, and explainability.

## Features

- Fake/Genuine classification API
- Batch review classification
- Basic review validation
- Frontend UI for review submission
- Model-based detection using text, behavioral, and fuzzy features

## Setup

### Backend

`powershell
cd Fake-Review-Detection-System/backend
python -m pip install -r requirements.txt
python -m uvicorn main:app --reload --port 8000
`

Open API docs at http://localhost:8000/docs.

### Frontend

`powershell
cd Fake-Review-Detection-System/frontend
npm install
npm run dev
`

Open the frontend at http://localhost:5173.

## Project structure

`
Fake-Review-Detection-System/
  backend/
    main.py
    requirements.txt
    model_bundle.pkl
    ...
  frontend/
    src/
      app.jsx
      main.jsx
    package.json
    vite.config.js
  Readme.md
  ieee_paper.md
  reviewscan_ieee_paper.md
`

## Notes

- The backend serves the classification API.
- The frontend calls the backend API to display fake review results.
- Model files are included for prediction, but training scripts are also available.

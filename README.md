# AI Mock Interview System

An AI-powered web application that simulates a real technical interview environment with automated evaluation, speech recognition, resume matching, and AI-based proctoring.

---

## 📌 Project Overview

The AI Mock Interview System is a full-stack web application designed to simulate structured technical interviews.

The system evaluates candidates using:

- 🎤 Real-time Speech Recognition
- 📄 Resume-to-Job Description Matching
- 👁 AI-Based Face Tracking & Focus Monitoring
- 📊 Automated Performance Scoring & Report Generation

It combines **Natural Language Processing (NLP)** and **Computer Vision** to create a structured, intelligent, and data-driven interview experience.

---

## 🎯 Objective

The goal of this project is to:

- Simulate structured technical interview scenarios
- Analyze candidate responses using NLP techniques
- Monitor candidate focus using computer vision
- Generate automated, weighted performance reports

---

## 🏗 System Architecture

The system is divided into five core components:

### 1️⃣ Frontend
- HTML
- CSS (Grid, Flexbox)
- JavaScript
- Web Speech API

### 2️⃣ Backend
- Flask (Python)
- REST APIs
- Session Management

### 3️⃣ NLP Processing
- Text Cleaning
- TF-IDF Vectorization
- Cosine Similarity
- Keyword-Based Answer Scoring

### 4️⃣ Proctoring Module
- MediaPipe Face Mesh
- Real-time Webcam Capture
- Focus Direction Detection (Left / Right / Down)
- Violation Counter Tracking

### 5️⃣ Storage
- Session-based Data Storage
- File Upload Handling (Resume & JD)

---

## ⚙️ Development Methodology

The system follows a structured implementation pipeline:

1. User uploads Resume and Job Description
2. Interview questions are simulated
3. Speech is captured and transcribed in real-time
4. Face focus is monitored using MediaPipe
5. NLP algorithms evaluate responses
6. Final weighted performance score is generated

---

## 🧠 Implementation Details

### 🎤 Speech Recognition

- Used Web Speech API
- Continuous transcription enabled
- Captured full interview transcript
- Stored transcript in session
- Sent final answer to backend using Fetch API

Example:

```javascript
recognition.continuous = true;
recognition.interimResults = true;
recognition.start();
```

---

### 📄 Resume Matching (NLP Module)

Steps:

- Cleaned resume and job description text
- Converted text into TF-IDF vectors
- Measured similarity using Cosine Similarity

Mathematically:

Similarity = cosine(angle between resume vector and job description vector)

This transforms textual similarity into a measurable numerical score.

---

### 📊 Scoring Logic

Final Score is calculated using weighted evaluation:

Final Score =  
(Answer Quality × 0.4) +  
(Confidence × 0.3) +  
(Integrity × 0.3)

Where:

- Answer Quality → Keyword relevance
- Confidence → Speech length & pause penalty
- Integrity → Focus violations detected

---

### 👁 Proctoring System

- Real-time webcam capture
- Face detection using MediaPipe
- Focus tracking (Left / Right / Down)
- Violation counter increments automatically
- Integrity score decreases based on violations

---

## ✨ Features Implemented

- Multi-question interview simulation
- Real-time speech-to-text transcription
- Resume & JD similarity scoring
- AI-based proctoring system
- Automated weighted performance report
- Clean UI with structured dashboard
- Session-based data handling

---

## 🛠 Technologies Used

### Frontend
- HTML
- CSS
- JavaScript
- Web Speech API

### Backend
- Flask
- Python

### AI / ML
- TF-IDF Vectorizer
- Cosine Similarity
- MediaPipe Face Mesh
- OpenCV (Browser Webcam)

---

## 📂 Project Structure

```
AI-Mock-Interview-System/
│
├── app.py
├── requirements.txt
├── templates/
│   ├── setup.html
│   ├── interview.html
│   └── result.html
│
├── static/
│   ├── style.css
│   ├── video_proctoring.js
│   └── images/
│
└── uploads/
```

---

## ▶️ Installation

1. Clone the repository:

```
git clone https://github.com/your-username/AI-Mock-Interview-System.git
```

2. Install dependencies:

```
pip install -r requirements.txt
```

3. Run the application:

```
python app.py
```

4. Open in browser:

```
http://127.0.0.1:5000
```

---

## 📸 Screenshots

### Interview Interface
(Add screenshot here)

### Performance Report
(Add screenshot here)

---

## 🔮 Future Improvements

- LLM-based semantic answer evaluation
- Emotion detection module
- Database integration
- Multi-user support
- Cloud deployment

---

## 👩‍💻 Author

Developed by Kareena Rohra  
B.Sc. Data Science Student  

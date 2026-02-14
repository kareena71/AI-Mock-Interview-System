#AI Mock Interview System
Overview

The AI Mock Interview System is a web-based application that simulates a real technical interview environment.

The system evaluates candidates using:

Real-time speech recognition

Resume-to-job-description matching

AI-based face tracking and proctoring

Automated performance scoring and report generation

It combines Natural Language Processing (NLP) and Computer Vision to create a structured, AI-driven interview experience.

Objective

The goal of this project is to:

Simulate structured technical interview scenarios

Analyze candidate responses using NLP

Monitor candidate focus using computer vision

Generate automated, data-driven performance reports

Approach

The system follows a modular architecture consisting of four major layers:

1️⃣ User Interface Layer

Handles:

Candidate profile setup

Interview interface

Live transcript display

Performance report visualization

2️⃣ Speech Processing Layer

Uses Web Speech API for real-time transcription

Captures continuous speech input

Maintains full interview transcript

Sends data to backend via Fetch API

3️⃣ NLP & Scoring Engine

Cleans text input

Converts resume & JD into TF-IDF vectors

Calculates similarity using Cosine Similarity

Evaluates answer quality based on keyword relevance

Computes final performance score

4️⃣ AI Proctoring Engine

Uses MediaPipe Face Mesh

Tracks face direction (Left / Right / Down)

Increments violation counter

Impacts integrity score

Features Implemented

User profile setup (Name, Role, Resume Upload, JD Upload)

Real-time speech-to-text transcription

Continuous interview recording

Resume & Job Description similarity scoring

AI-based face detection and tracking

Focus violation monitoring

Integrity scoring system

Automated final score calculation

Structured performance report dashboard

Scoring Logic

Final Score =
(Answer Quality × 0.4) +
(Confidence × 0.3) +
(Integrity × 0.3)

Metrics Explained:

Answer Quality
→ Based on keyword relevance and structure.

Confidence
→ Based on speech length and pauses.

Integrity
→ Based on focus violations during interview.

Technologies Used
Frontend

HTML

CSS (Flexbox, Grid)

JavaScript

Web Speech API

Backend

Python

Flask

REST APIs

Session Management

NLP / Data Science

TF-IDF Vectorizer (scikit-learn)

Cosine Similarity

Text Preprocessing

Computer Vision

MediaPipe Face Mesh

Webcam integration via browser

System Architecture

User → Frontend Interface →
Speech Recognition + Webcam →
Flask Backend →
NLP Processing + Proctoring Logic →
Score Calculation →
Performance Report

Project Structure:
AI-Mock-Interview-System/
│
├── app.py
├── uploads/
│
├── templates/
│   ├── setup.html
│   ├── interview.html
│   └── result.html
│
├── static/
│   ├── style.css
│   ├── video_proctoring.js
│   └── ai_assistant.png
│
└── README.md

Components Included

Speech recognition module

Resume similarity module

Scoring algorithm module

Proctoring detection module

Flask backend routing

UI layout and styling

Performance analytics report

Future Enhancements

Integration with advanced LLMs for semantic answer evaluation

Database integration (PostgreSQL / MongoDB)

Multi-question dynamic interview sets

Cloud deployment (AWS / Render)

Admin analytics dashboard

Conclusion

This project demonstrates the integration of:

Web development

Natural Language Processing

Machine Learning similarity metrics

Real-time computer vision monitoring

Automated scoring systems

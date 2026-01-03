# AI Video Summarizer

An AI-powered web application that automatically converts long videos into concise and meaningful summaries using modern Speech Recognition and Natural Language Processing models.

---

## Current Features (Implemented)

- Upload video files (MP4)
- High-accuracy speech-to-text using OpenAI Whisper
- Abstractive text summarization using BART
- Speaker diarization using pyannote.audio
- Visual keyframe extraction using OpenCV
- Clean text summary and full transcript
- Simple, responsive frontend

---

## Tech Stack (Current)

## Frontend
- React.js
- Vite
- Tailwind CSS

### Backend
- Python
- FastAPI

### AI / ML
- OpenAI Whisper (ASR)
- BART (`facebook`)
- Hugging Face Transformers
- Pyannote.audio (Speaker Diarization)
- OpenCV (Keyframe Extraction)

---

## Application Workflow

1. User uploads a video file
2. Backend extracts audio from the video
3. Whisper converts audio to text
4. Transcript is cleaned and chunked
5. BART generates an abstractive summary
6. OpenCV extracts keyframes
7. Results are sent back to the frontend

---
## Structure
```
AI-video_summarizer/
├── backend/
│ ├── utils/
│ ├── main.py
│ ├── requirements.txt
│ └── .env.example
│
├── frontend/
│ ├── public/
│ ├── src/
│ ├── index.html
│ ├── package.json
│ └── vite.config.js
│
├── .gitignore
└── README.md
```
---
## Screenshots
### Frontend
![frontend](https://github.com/user-attachments/assets/d7104ccb-dc25-45a3-8d44-19edaafedec1)

### Output
![output](https://github.com/user-attachments/assets/01d844e4-b308-4edb-8154-972287f0fa2b)

---

## Installation & Execution

### 1. Clone the Repository
```bash
git clone https://github.com/Dhirajsah18/AI-video_summarizer.git
cd AI-video_summarizer
```
### 2. Backend Setup
```bash
cd backend
python -m venv venv
source venv/bin/activate   # Windows: venv\Scripts\activate
pip install -r requirements.txt
uvicorn main:app --reload

```
### 3. Frontend Setup
```bash
cd frontend
npm install
npm run dev

```

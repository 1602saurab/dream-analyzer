# 🌙 Dream Journal Analyzer — Multi-Agent System

Built with **LangGraph** + **Gemini 2.5 Flash**

## Project Structure
```
dream_analyzer/
├── agents.py      ← LangGraph multi-agent pipeline
├── app.py         ← Flask server
├── index.html     ← Full frontend (single file)
└── README.md
```

## Agents (LangGraph Pipeline)
```
User Input
    ↓
Emotion Detector  →  Symbol Decoder  →  Pattern Tracker  →  Insight Narrator
                                                                    ↓
                                                            Dream Report
```

## Setup & Run

### 1. Install dependencies
```bash
pip install langgraph langchain-google-genai flask flask-cors
```

### 2. Get a Gemini API Key
- Go to https://aistudio.google.com/apikey
- Create a free API key

### 3. Run the server
```bash
cd dream_analyzer
python app.py
```

### 4. Open the app
Visit: http://localhost:5000

### 5. Use it
- Paste your Gemini API key in the field
- Describe your dream
- Click **Analyze My Dream**

# Emotion Detection Web Application

A full-stack AI-based web application developed as part of the IBM / Coursera course **"Developing AI Applications with Python and Flask"**.

The application utilizes IBM Watson NLP's EmotionPredict service to analyze user-submitted text and detect five core emotions: **anger**, **disgust**, **fear**, **joy**, and **sadness**, while also identifying the **dominant emotion**.

---

## 🚀 Features

- **Emotion Detection Engine**: Communicates with Watson NLP to compute confidence scores for five emotional dimensions.
- **Output Formatting**: Parses Watson NLP responses into structured dictionaries with dominant emotion extraction.
- **Python Packaging**: Encapsulated within the reusable `EmotionDetection` package.
- **Unit Testing**: Automated test suite (`test_emotion_detection.py`) validating emotional classifications.
- **Flask Web Deployment**: Interactive web user interface (`server.py`) rendering real-time sentiment results.
- **Error Handling**: Gracefully handles blank or invalid inputs (HTTP 400) with descriptive messages.
- **PEP 8 / Static Code Analysis**: 100% compliant with pylint standards (rated at 10.00/10).

---

## 🛠️ Project Structure

```text
oaqjp-final-project-emb-ai/
├── EmotionDetection/
│   ├── __init__.py            # Package initialization exposing emotion_detector
│   └── emotion_detection.py   # Watson NLP EmotionPredict API integration
├── static/
│   └── mywebscript.js         # Frontend asynchronous AJAX request logic
├── templates/
│   └── index.html             # Responsive Bootstrap UI template
├── server.py                  # Flask server and routing endpoints
├── test_emotion_detection.py  # Unit test suite
└── README.md
```

---

## 💻 Running the Application

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/nguyenvietnhan/oaqjp-final-project-emb-ai.git
   cd oaqjp-final-project-emb-ai
   ```

2. **Install Dependencies**:
   ```bash
   pip install requests flask pylint
   ```

3. **Run Unit Tests**:
   ```bash
   python test_emotion_detection.py
   ```

4. **Start the Flask Server**:
   ```bash
   python server.py
   ```
   Open your browser and navigate to `http://localhost:5000`.

---

## 📄 License

This project is licensed under the Apache License 2.0.

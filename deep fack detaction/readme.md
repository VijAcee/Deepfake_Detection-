# AI-Based Real/Fake Image Detection and Live Face Mapping System

A comprehensive web application that uses artificial intelligence to detect manipulated images and perform real-time face mapping with secure user authentication.

## 🎯 Features

- **User Authentication**: Secure login and registration system
- **Real/Fake Image Detection**: AI-powered detection using deep learning
- **Live Face Mapping**: Real-time face detection and mapping
- **Detection History**: Store and view all detection results
- **User Dashboard**: Easy-to-use interface with two main options
- **Responsive Design**: Works on desktop and mobile devices

## 🛠️ Tech Stack

- **Backend**: Flask (Python)
- **AI/ML**: TensorFlow, OpenCV
- **Frontend**: HTML5, Bootstrap 4, JavaScript
- **Database**: SQLite
- **Image Processing**: OpenCV, Pillow

## 📋 Prerequisites

- Python 3.7+
- pip (Python package manager)
- Webcam (for face mapping feature)

## 🚀 Installation & Setup

### 1. Clone Repository
```bash
git clone https://github.com/yourusername/ai-image-detection-system.git
cd ai-image-detection-system
```

### 2. Create Virtual Environment
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

### 3. Install Dependencies
```bash
pip install -r requirements.txt
```

### 4. Create Database
```bash
python
>>> from models import Database
>>> db = Database()
>>> exit()
```

### 5. Run Application
```bash
python app.py
```

### 6. Access Application
Open your browser and go to: `http://localhost:5000`

## 📁 Project Structure

```
ai-image-detection-system/
├── app.py                 # Main Flask application
├── config.py              # Configuration file
├── requirements.txt       # Dependencies
├── database.db            # SQLite database
├── models/
│   ├── __init__.py
│   ├── database.py       # Database operations
│   ├── detection.py      # Image detection model
│   └── face_mapping.py   # Face mapping model
├── static/
│   ├── styles.css        # CSS styling
│   ├── uploads/          # Uploaded images
│   └── js/
│       └── face_detection.js
└── templates/
    ├── base.html
    ├── login.html
    ├── register.html
    ├── dashboard.html
    ├── detect.html
    ├── mapping.html
    ├── history.html
    └── profile.html
```

## 📖 Usage

### 1. Registration
- Go to registration page
- Enter username, password, and email (optional)
- Click Register

### 2. Login
- Enter credentials
- Click Login to access dashboard

### 3. Image Detection
- Click "Real/Fake Image Detection"
- Upload an image
- Get AI-powered prediction result

### 4. Face Mapping
- Click "Live Face Mapping"
- Choose webcam or upload image
- Detect faces in real-time

### 5. View History
- Click "History" in navigation
- See all detection records
- Delete records if needed

## 🔐 Security Features

- Password encryption (for production, implement bcrypt)
- Session management
- File upload validation
- CSRF protection with Flask sessions
- Input validation and sanitization

## 🎓 Project Objectives

✅ Detect fake/manipulated images using AI
✅ Perform real-time face mapping
✅ Provide secure login system
✅ Store user detection history
✅ User-friendly web interface
✅ Demonstrate AI in image processing

## 📊 System Architecture

```
User Interface Layer (HTML, CSS, JavaScript)
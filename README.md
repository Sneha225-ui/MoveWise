# 🧍 MoveWise – AI-Powered Movement & Posture Coach

**Smarter guidance for every movement.**

MoveWise is an AI-powered movement and posture coaching application designed to help users improve their exercise technique through real-time pose detection, personalized feedback, and movement analysis.

Using computer vision and adaptive coaching, MoveWise analyzes body movements, identifies posture mistakes, provides corrective guidance, and tracks exercise progress.

The goal is simple: **make movement guidance smarter, more accessible, and personalized.**

---

## ✨ Features

### 1. AI-Powered Exercise Recognition
- Automatically recognizes supported exercises.
- Uses computer vision and pose detection.
- Supports webcam and video-based movement analysis.

### 2. Exercise Library

MoveWise currently supports four exercises:

| Category | Exercise |
|---|---|
| Yoga | Warrior II |
| Yoga | Tree Pose |
| Fitness | Squat |
| Fitness | Bicep Curl |

### 3. Real-Time Posture Analysis
- Detects body landmarks.
- Analyzes posture and movement.
- Identifies common exercise form mistakes.
- Provides corrective feedback during exercise sessions.

### 4. Ghost Coach 👻
- Displays a reference movement guide.
- Helps users understand correct body alignment.
- Uses visual guidance and correction arrows.

### 5. Adaptive Coaching
- Prioritizes important posture corrections.
- Adjusts coaching instructions based on movement performance.
- Provides easier exercise variations when needed.
- Includes comfort feedback to make coaching more user-friendly.

### 6. Personal Body Map
- Adapts movement analysis to the landmarks that can be tracked.
- Supports Standard and Adaptive analysis modes.
- Avoids treating untracked body landmarks as incorrect posture.

### 7. Exercise Tracking & Progress
- Tracks exercise sessions and performance.
- Records repetitions and movement scores where applicable.
- Provides session summaries.
- Helps users review their exercise history and progress.

### 8. User Authentication & Profiles
- User registration and login.
- Password hashing using bcrypt.
- Personal profile information.
- SQLite-based user and exercise record storage.

---

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Python | Core application development |
| Streamlit | Interactive web application |
| OpenCV | Camera and video processing |
| MediaPipe | Human pose landmark detection |
| NumPy | Numerical computations |
| SQLite | User and exercise data storage |
| bcrypt | Password hashing |

---

## 🏗️ Project Structure

```text
MoveWise/
│
├── app.py
├── db_handler.py
├── requirements.txt
├── README.md
├── run.bat
├── package.py
├── export_samples.py
│
├── core/
│   ├── engine.py
│   ├── detector.py
│   ├── landmarks.py
│   ├── smoothing.py
│   ├── scoring.py
│   ├── coaching.py
│   ├── motion.py
│   ├── bodymap.py
│   ├── bodygroups.py
│   ├── phases.py
│   ├── reference.py
│   ├── session.py
│   ├── storage.py
│   └── synthetic.py
│
├── exercises/
│   ├── base.py
│   ├── registry.py
│   ├── warrior2.py
│   ├── tree_pose.py
│   ├── squat.py
│   └── bicep_curl.py
│
├── ui/
│   ├── theme.py
│   └── overlay.py
│
├── models/
│   └── pose_landmarker_lite.task
│
├── data/
│
└── test_*.py
```

---

## ⚙️ Installation & Setup

### Prerequisites

- Python 3.10 or a compatible Python version.
- Git.
- Webcam (optional if using sample clips or video input).

### Step 1: Clone the repository

```bash
git clone https://github.com/Sneha225-ui/Move-Wise.git
```

### Step 2: Navigate to the project folder

```bash
cd Move-Wise
```

### Step 3: Create a virtual environment

```bash
python -m venv venv
```

Activate it on Windows:

```bash
venv\Scripts\activate
```

### Step 4: Install dependencies

```bash
pip install -r requirements.txt
```

### Step 5: Run the application

```bash
streamlit run app.py
```

The application will open in your browser.

**Alternative:** Windows users can also run `run.bat`.

---

## 🧪 Testing

MoveWise includes test suites for different application components.

Run individual tests using:

```bash
python test_pipeline.py
python test_clips.py
python test_analysis.py
python test_coaching.py
python test_session.py
python test_accessibility.py
python test_motion.py
python test_progress.py
python test_robust.py
```

These tests cover pose processing, exercise analysis, coaching, movement control, accessibility, session recording, and progress tracking.

---

## 🔄 How MoveWise Works

```text
User Input
    |
    v
Camera / Video / Sample Clip
    |
    v
Pose Detection
    |
    v
Body Landmark Extraction
    |
    v
Movement & Posture Analysis
    |
    v
Exercise Recognition
    |
    v
Adaptive Coaching
    |
    v
Visual Feedback & Ghost Coach
    |
    v
Session Summary
    |
    v
Progress Tracking
```

---

## 🛡️ Safety & Disclaimer

MoveWise is designed for general fitness and movement guidance.

- It is not a medical diagnostic tool.
- It does not replace professional medical advice or physiotherapy.
- Users should stop exercising if they experience pain or discomfort.
- Exercise feedback should be used as general guidance, not as a guarantee of injury prevention.

---

## 🚀 Future Scope

Potential future improvements include:

- Support for additional exercises.
- More personalized exercise recommendations.
- Enhanced movement analysis.
- Improved progress visualizations.
- Expanded accessibility features.
- More advanced AI-based coaching.

---

## 👩‍💻 Developer

Sneha Singh Chauhan

Project: **MoveWise – AI-Powered Movement & Posture Coach**

GitHub: https://github.com/Sneha225-ui

---

⭐ If you find MoveWise interesting, consider giving the repository a star!

**MoveWise – Don't adapt your body to the AI. Let the AI adapt to you.**

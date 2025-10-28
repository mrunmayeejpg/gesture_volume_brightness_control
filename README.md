✋ Hand Gesture Volume & Brightness Controller
🧠 Overview

This project uses MediaPipe and OpenCV to track hand landmarks through your webcam.
By detecting the distance between the thumb and index finger, it automatically adjusts system volume and screen brightness — no keyboard or mouse needed!

⚙️ Features

🎥 Real-time hand tracking using MediaPipe Hands

🔊 Control system volume with gestures

💡 Control screen brightness dynamically

🖐️ Smooth fingertip landmark tracking with visual feedback

🧩 Works offline after initial setup

🧩 How It Works
Gesture	Action
✋ Thumb and Index apart	Volume Up + Brightness High
🤏 Thumb and Index close	Volume Down + Brightness Low

The program continuously calculates the distance between the thumb tip (ID 4) and index finger tip (ID 8).
It adjusts volume and brightness based on that distance in real time.

🛠️ Technologies Used

Python 3.x

OpenCV (cv2) – for webcam and image handling

MediaPipe – for hand landmark detection

PyAutoGUI – to send system key presses (for volume)

Screen-Brightness-Control (SBC) – for managing brightness

🚀 Installation
1️⃣ Clone the repository
git clone https://github.com/<your-username>/hand-gesture-volume-brightness.git
cd hand-gesture-volume-brightness

2️⃣ Install dependencies
pip install opencv-python mediapipe pyautogui screen-brightness-control


(If you don’t have pip, install it using python -m ensurepip)

▶️ Usage
Run the program:
python hand_control.py

Controls:

Move your thumb and index apart → Volume Up + Brightness ↑

Bring them close → Volume Down + Brightness ↓

Press Esc to exit

📸 Visual Reference

While running, the program:

Draws hand landmarks (colored dots and lines)

Shows real-time webcam feed

Displays connecting lines between fingertips for visual feedback

⚠️ Notes

Works best in well-lit environments.

Keep your hand in frame for stable tracking.

Some systems may require admin privileges for brightness control.

💡 Future Improvements

Add gesture to mute/unmute.

Add on-screen display of volume/brightness levels.

Multi-hand gesture support.

Adjustable sensitivity for gesture detection.

👩‍💻 Author

Mrunmayee Kulat
AI & Robotics Enthusiast | Gesture Recognition | Human-Computer Interaction

# AI Proctor

## Overview
The **AI Proctor** is an AI-powered project designed to detect suspicious activities during online or offline examinations. It utilizes computer vision techniques to track head movements, eye gaze direction, and mobile phone usage in real-time.

## Features
- **Head Pose Estimation**: Detects head movements (e.g., looking up, down, left, right).
- **Eye Movement Tracking**: Monitors gaze direction to identify focus deviation.
- **Mobile Phone Detection**: Identifies unauthorized mobile phone usage.
- **Automated Logging**: Captures and stores screenshots of detected suspicious behavior.

## Tools & Technologies Used
- **Programming Language**: Python
- **Libraries & Frameworks**: OpenCV, MediaPipe, PyTorch, NumPy
- **Deep Learning Models**: Face Detection, Head Pose Estimation, Eye Tracking
- **Hardware**: Laptop Webcam (or External Camera)
- **Logging & Storage**: CSV/JSON for logs, Screenshot Saving

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/ParthYuki/AI_proctor.git
   cd AI_proctor
   ```
2. Ensure you have the necessary model files inside the `models` folder:
   - `best.pt`
   - `shape_predictor_68_face_landmarks.dat`

## Usage
Run the main script to start the surveillance system:
```bash
python main.py
```

## Project Structure
```
Cheating-Surveillance-System/
│── models/                  # Pretrained models for detection
│   ├── best.pt              # Model for head pose estimation and object detection
│   ├── shape_predictor_68_face_landmarks.dat # Landmark detection model
│── log/                     # Stored screenshots of detected activities
│── eye_movement.py          # Eye movement detection logic
│── head_pose.py             # Head pose estimation
│── main.py                  # Main execution script
│── mobile_detection.py      # Mobile phone detection logic
│── README.md                # Project documentation
```

## Logs & Screenshots
Detected suspicious activities are stored in the `log/` folder with timestamped images.

## Future Improvements
- Improve model accuracy with more training data.
- Implement audio alerts for detected violations.
- Enhance real-time processing efficiency.

## Contributing
Feel free to open issues or submit pull requests to improve the project!

🖐️ **Virtual Mouse Using Hand Gestures**

A computer vision–based virtual mouse system that allows users to control mouse movement and actions using hand gestures captured via a webcam. The project demonstrates touch-free human–computer interaction using real-time hand tracking.
---

## Features
* Mouse movement using index finger tracking
* Left click using finger gesture
* Right click using finger gesture
* Double click support
* Screenshot capture using hand gesture
* Gesture debouncing to prevent repeated clicks
* Real-time performance
---

## Tech Stack
* Python 3
* OpenCV
* MediaPipe Hands
* NumPy
* Pynput
* PyAutoGUI
---

## Project Structure

```
virtual-mouse/
├── virtual_mouse.py
├── util.py
├── README.md
```
---

## Gesture Mapping

| Gesture               | Action       |
| --------------------- | ------------ |
| Index finger movement | Move cursor  |
| Index finger bent     | Left click   |
| Middle finger bent    | Right click  |
| Index + Middle bent   | Double click |
| Pinch gesture         | Screenshot   |
---

## Installation

```bash
pip install opencv-python mediapipe numpy pynput pyautogui
## Run the Project
```bash
python virtual_mouse.py
```
* Ensure your webcam is connected
* Press `Q` to exit

---

## How It Works
* MediaPipe detects 21 hand landmarks
* Finger joint angles are calculated to identify gestures
* Distance between thumb and index finger is used for pinch detection
* Gestures are mapped to mouse events using Pynput
* Click debouncing prevents system freeze
---

## Notes
* Works best in good lighting
* Supports single-hand operation
* Keep hand within camera frame
---

## Future Enhancements
* Scroll gestures
* Cursor smoothing
* Multi-hand support
* Custom gesture mapping
---

## Author
Sai Sonawane


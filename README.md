# 🚗 Real-Time Vehicle Detection

A Python-based application for real-time vehicle detection, counting, and analysis using YOLOv8, designed to process video streams and output traffic insights.

---

## 🧰 Table of Contents

- [About the Project](#about-the-project)  
- [Features](#features)  
- [Demo](#demo)  
- [Installation](#installation)  
- [Usage](#usage)  
- [Project Structure](#project-structure)  
- [Dependencies](#dependencies)  
- [Contributing](#contributing)  
- [License](#license)  
- [Contact](#contact)  

---

## About the Project

This repository provides a lightweight, efficient pipeline for detecting vehicles in real-time from video feeds:

1. **Detection** – Uses YOLOv8 (via a pre-trained `yolov8n.pt` model).
2. **Analysis** – Processes bounding boxes to count vehicles, log occurrences, and estimate traffic flow.
3. **Integration** – Outputs metrics to CSV, enabling further visualization or dashboard integration.

Perfect for traffic monitoring, smart city applications, and ITS enthusiasts.

---

## Features

- **Real-time object detection** of cars, motorcycles, buses, etc.  
- **Count & track** vehicles across frames using `sort.py`.  
- **Export statistics** to a CSV (`traffic_stats.csv`).  
- **Process local video files** (e.g., `simple.mp4`).  

---

## Demo

See it in action:

bash
python trafficAnalyzer.py --video simple.mp4 --output traffic_stats.csv
This runs detection, tracks vehicles, and saves stats to CSV.

Installation
Clone the repo

bash
Copy
Edit
git clone https://github.com/Aniket-Paul1/Real_Time_Vehicle_Detection.git
cd Real_Time_Vehicle_Detection
Install dependencies

bash
Copy
Edit
pip install -r requirements.txt
Note: If requirements.txt isn't provided, the key Python packages are:

bash
Copy
Edit
pip install ultralytics opencv-python scipy pandas sort-tracker
Download the YOLOv8 model
The repo already includes a lightweight yolov8n.pt model for detection.

Usage
Detect from a video file
bash
Copy
Edit
python trafficAnalyzer.py \
  --video simple.mp4 \
  --weights yolov8n.pt \
  --output traffic_stats.csv \
  --show
--show: display detection in a real-time window (optional).

Output metrics (e.g., frame count, total vehicles) saved to CSV.

Customize tracking
Use sort.py directly if you want to integrate the SORT tracker in your own application.

🗂 Project Structure
bash
Copy
Edit
Real_Time_Vehicle_Detection/
├── __pycache__/            # Python bytecode cache
├── sort.py                 # SORT tracking implementation
├── trafficAnalyzer.py      # Main detection & tracking script
├── simple.mp4              # Sample video for testing
├── yolov8n.pt              # YOLOv8 nano pretrained model
├── traffic_stats.csv       # Sample output file
├── requirements.txt        # Python dependencies
└── README.md               # (this file)
🔧 Dependencies
Python 3.7+

ultralytics – for YOLOv8

OpenCV (opencv-python) – video processing

SORT tracker or equivalent (sort-tracker)

Pandas – for exporting results to CSV

Contributing
Contributions are very welcome! Feel free to:

Improve detection accuracy (e.g., retraining, new YOLO weights)

Add functionality (e.g., speed estimation, license plate recognition)

Convert into a production-ready service (API, Docker container, etc.)

To contribute:

Fork the repository

Create a feature branch (git checkout -b my-feature)

Commit your changes (git commit -m "Add my feature")

Push to the branch (git push origin my-feature)

Create a Pull Request

License
Distributed under the MIT License. See LICENSE file for details.

📬 Contact
For questions or feedback, feel free to reach out:

Aniket Paul – [YourEmail@example.com]

Built with passion and code. Happy detecting! 🚦

makefile
Copy
Edit
::contentReference[oaicite:0]{index=0}

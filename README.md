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

```bash
python trafficAnalyzer.py --video simple.mp4 --output traffic_stats.csv
```
---

## Installation

1. **Clone the repository**  
   ```bash
   git clone https://github.com/Aniket-Paul1/Real_Time_Vehicle_Detection.git
   cd Real_Time_Vehicle_Detection
   ```
   

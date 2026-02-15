# 🚗 Vehicle Counting using YOLOv8 and YOLOv10

## 📌 Overview

This project presents a comparative study of **YOLOv8** and **YOLOv10** combined with **ByteTrack** and **DeepSORT** for real-time vehicle detection and counting in traffic surveillance videos.

The goal is to evaluate detection accuracy, tracking stability, and ID consistency across different detector–tracker combinations.

---

## 🧠 Methodology

### 🔹 Object Detection
- YOLOv8  
- YOLOv10  

### 🔹 Multi-Object Tracking
- ByteTrack  
- DeepSORT  

### 🔹 Pipeline

1. Input traffic video  
2. Detect vehicles using YOLO  
3. Track vehicles across frames  
4. Count vehicles crossing a predefined line  
5. Output annotated video with ID tracking and counting statistics  

---

## 📊 Model Combinations

| Detector | Tracker   |
|----------|------------|
| YOLOv8   | ByteTrack  |
| YOLOv8   | DeepSORT   |
| YOLOv10  | ByteTrack  |
| YOLOv10  | DeepSORT   |

---

## 🎥 Demo Results

Example output videos:

- `output_v8_bytetrack.mp4`
- `output_v8_deepsort.mp4`
- `output_v10_bytetrack.mp4`
- `output_v10_deepsort.mp4`

Combined comparison video:

- `compare_yolov8_vs_yolov10.mp4`

---

## 📈 Observations

- YOLOv10 shows improved detection confidence in complex traffic scenes.
- ByteTrack provides more stable ID assignment under moderate occlusion.
- DeepSORT reduces ID switches in dense vehicle scenarios.
- YOLOv10 + ByteTrack demonstrates the best balance between speed and tracking consistency.



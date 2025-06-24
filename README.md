# Player Re-Identification in a Single Camera Feed (Task 2)

This repository contains a complete implementation for **Player Re-Identification in a Single Feed** using YOLOv5 and Deep SORT tracking. It was developed as part of the AI Internship Assignment at **Liat.ai**.

## Task Objective

Given a 15-second video (`15sec_input_720p.mp4`), the goal is to:

- Detect all players using a provided YOLOv11 model.
- Assign unique IDs to each player during the initial seconds.
- Track and retain those IDs for each player, even if they leave and re-enter the frame later.

## Technologies Used

- Python 3.12
- OpenCV
- PyTorch
- Ultralytics YOLOv5 (custom model `yolov11.pt`)
- Deep SORT Realtime (`deep_sort_realtime`)
- Matplotlib, Ipywidgets (for interactive visualization)

## How It Works

1. The YOLOv11 model is used to detect "players" in each frame.
2. Deep SORT is used to track these players across time.
3. Player IDs are maintained even if they temporarily exit the frame.
4. A frame viewer (slider) allows visual inspection of player IDs.
5. An annotated output video is saved (`output_video.mp4`).

## 📦 Installation

Clone the repository and install required libraries:
pip install -r requirements.txt

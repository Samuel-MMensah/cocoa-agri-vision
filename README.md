# Cocoa Agri-Vision
Fine-grained cocoa disease detection with per-frame pod counting.

## Problem
Cocoa farmers lose 30–40% of yield to black pod rot. Manual inspection is slow and subjective. This system detects diseased pods in real time from field images.

## Approach
- Custom dataset collected on a working cocoa farm (500+ images)
- YOLOv11 object detection trained on annotated pod data
- Per-frame disease prevalence estimation
- Edge deployment targeting Jetson Orin Nano

## Results
| Model | mAP@50 | mAP@50:95 | FPS (T4 GPU) |
|-------|--------|-----------|--------------|
| yolo11n baseline | — | — | — |

## Quick Start
```bash
git clone https://github.com/Samuel-MMensah/cocoa-agri-vision.git
pip install ultralytics
yolo detect train data=configs/data.yaml model=yolo11n.pt epochs=50

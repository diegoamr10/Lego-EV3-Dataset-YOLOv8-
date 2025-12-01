# LEGO EV3 Object Detection Dataset for YOLOv8
This repository contains a custom dataset designed for training and evaluating YOLOv8 object detection models using images of LEGO EV3 robots.
The dataset was created specifically for computer vision experiments, robotic tracking, and the study of chaotic trajectories such as the Rössler and Lorenz systems.

---

## 📂 Dataset Description
The dataset includes:

- **High-resolution images** of a LEGO EV3 robot from different angles.
- **Multiple lighting conditions** and backgrounds.
- **Annotated bounding boxes** following YOLO format.
- **Consistent class labeling**, ideal for training detection models.
  
This dataset is suitable for:
- Robot tracking projects  
- Real-time object detection  
- Machine learning experiments with LEGO robotics  
- YOLOv5/YOLOv8 training pipelines  

---

## 🏷 Classes
The dataset currently includes the following class:
- Lego (Mindstorm EV3 Brick)

---
### 🚀 Usage
git clone [https://github.com/tu-repo/lego-ev3-dataset.git](https://github.com/diegoamr10/DifferentialRobot-LegoEV3-YOLOv8-Dataset.git
cd lego-ev3-dataset
pip install ultralytics
yolo detect train data=dataset.yaml model=yolov8m.pt epochs=100 imgsz=640
  Where:
    dataset.yaml contains the paths to the train/val folders and class names

  yolov8n.pt can be replaced with yolov8s.pt, yolov8m.pt, etc.

Using the Trained Model (best.pt)
  yolo detect predict model=best.pt source=folder_or_video
---

## 👥 Authors
D. A. Mata Robles, R. C. Martínez-Montejano, R. C. Martínez-Montejano, J. J. Jaime-Rodriguez

--- 

## 🙌 Acknowledgments
D.A.M.R and L.J.O.G. thank the Potosino Council of Science and Technology (COPOCYT) for the support provided through Trust Project 23871, from the 2023-01 Call.
---

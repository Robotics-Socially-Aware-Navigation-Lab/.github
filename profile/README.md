<p align="center">
  <img src="https://github.com/Robotics-Socially-Aware-Navigation-Lab/.github/assets/lab_logo.png" width="220" alt="RSAN Lab Logo"><br>
  <h1 align="center">🤖 Robotics Socially Aware Navigation Lab (RSAN Lab)</h1>
  <h3 align="center">Making Robots Socially Intelligent</h3>
</p>

---

<p align="center">
  <b>Department of Computer Science — Sonoma State University</b><br>
  <a href="https://github.com/Robotics-Socially-Aware-Navigation-Lab">🌐 github.com/Robotics-Socially-Aware-Navigation-Lab</a>
</p>

---

## Overview

The **Robotics Socially Aware Navigation Lab (RSAN Lab)** was established to advance research and development in **socially aware robotic navigation**, combining **computer vision**, **machine learning**, and **robotic reasoning** to create **context-aware autonomous systems**.

The **RSAN_Project** is the flagship system developed for *CS470: Advanced Software Design Project* at **Sonoma State University (SSU)**.  
This project represents a collaborative effort by a multidisciplinary team focused on the intersection of **AI perception**, **Large Language Models (LLMs)**, and **robotic navigation** using **ROS2**.

Through a modular, research-driven design, the system integrates **perception**, **reasoning**, and **navigation** to enable robots to interpret human-centric environments and respond appropriately.  
This work exemplifies advanced concepts in **object detection**, **scene understanding**, **contextual inference**, and **behavior-based robotics**.

---

## System Overview

The **SAN_Project Robot Production Pipeline** consists of modular components, each serving a unique role within the robot intelligence framework.

### Data Collection & Cleaning
- Gathers and refines real-world or simulated datasets (**COCO**, **SUN RGB-D**).  
- Processes image data to remove noise and ensure balanced training samples.  
- **Implemented in:**
  - `colab/preprocess_data.ipynb`
  - `src/perception/preprocess_data.py`

### Model Training (YOLOv9)
- Fine-tunes YOLOv9 on custom datasets for **human-object interaction recognition**.  
- Integrates social cues into object detection for **contextual awareness**.  
- **Implemented in:**
  - `colab/train_yolov9.ipynb`
  - `src/perception/train_yolo.py`

### Visual Perception & Detection
- Runs trained models to detect **people, objects, and obstacles**.  
- Supports both static images and **video streams** for real-time inference.  
- **Implemented in:**
  - `src/perception/detect_objects.py`

### LLM-Based Reasoning (ChatGPT-Vision Integration)
- Uses GPT-based models for **scene interpretation** and **semantic reasoning**.  
- Converts visual detections into **natural language context** for decision-making.  
- **Implemented in:**
  - `src/reasoning/llm_reasoner.py`
  - `src/reasoning/rule_engine.py`

### Navigation & Behavior Control (ROS2 Integration)
- Translates high-level reasoning into **low-level motion commands**.  
- Uses ROS2 topics to manage **path planning** and **robot control**.  
- **Implemented in:**
  - `src/navigation/ros2_interface.py`
  - `src/navigation/san_behavior.py`

### Evaluation & Documentation
- Tracks **model performance** and **robot behavior metrics**.  
- Produces **reports**, **visualizations**, and **reproducible results**.  
- **Implemented in:**
  - `docs/model_training.md`
  - `results/logs/`

---

## Research Motivation

Modern robotics must extend beyond navigation — it must **understand and adapt to social contexts**.  
The **RSAN_Project** explores the fusion of **visual perception** and **language-based reasoning** to empower robots to:

- Recognize **people**, **gestures**, and **environments**  
- Understand **contextual meaning** in scenes  
- Navigate **safely and respectfully** in human spaces  

This layered design mirrors how humans combine **sight, reasoning, and decision-making** —  
a key step toward **socially intelligent autonomous systems**.

---

## Technologies and Frameworks

| Domain | Tool / Framework | Purpose |
|--------|------------------|----------|
| **Computer Vision** | YOLOv9 / OpenCV | Object detection and real-time inference |
| **Dataset Management** | FiftyOne / Albumentations | Data cleaning, augmentation, and visualization |
| **Reasoning** | ChatGPT-Vision / LangChain | Semantic interpretation of detected scenes |
| **Robotics** | ROS2 (Humble) | Real-world control and sensor integration |
| **ML Workflow** | Python, PyTorch, Jupyter, Colab | Model training and experimentation |

---

## Contributors


---

## Institution

Developed at the **Department of Computer Science**,  
**Sonoma State University**, Rohnert Park, California, USA.

---

<p align="center">
  <b>© 2025 Robotics Socially Aware Navigation Lab (RSAN Lab)</b><br>
  Sonoma State University — Department of Computer Science  
  <br><br>
  <a href="https://github.com/Robotics-Socially-Aware-Navigation-Lab">
    🔗 Visit the RSAN Lab on GitHub
  </a>
</p>

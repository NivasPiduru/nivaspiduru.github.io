---
title: "Voice-Controlled Robotic Manipulation System"
excerpt: "AI-powered robot responding to natural language voice commands with computer vision and LLM integration"
collection: portfolio
date: 2025-12-01
---
## Project Links
* **GitHub Repository**: [View Code](https://github.com/NivasPiduru/voice-controlled-robot) 
* **Video Demo**: [Watch Demo](https://youtu.be/byuuGB1L9Vg)

## Overview
Developed an autonomous robotic manipulation system that responds to natural language voice commands, integrating computer vision, LLM-based parsing, and real-time robot control. The system enables non-technical users to control complex robotic tasks through simple voice commands like "stack the red block on the blue one."

## Key Features
* **Wake Word Detection**: Hands-free activation using "hey robot" trigger phrase
* **Vision-Based Perception**: Real-time object detection with OpenCV for 4DOF pose estimation and spatial reasoning
* **Natural Language Understanding**: Google Gemini 2.5 Flash LLM parses complex multi-step commands into executable robot actions
* **Intelligent Control**: Dynamic Z-height adjustment, rotation matching, multi-level stacking, and collision avoidance algorithms

## Technical Implementation

### Architecture
Built modular ROS2 (Humble) architecture with five independent publisher-subscriber nodes:
- **Vision Detector Node**: Computer vision processing and object detection
- **LLM Parser Node**: Natural language command interpretation with spatial reasoning
- **Coordinate Converter Node**: Homography-based pixel-to-robot coordinate transformation
- **Executor Node**: Robot motion planning and control
- **Voice Command Node**: Speech recognition and wake word detection

### Technologies Used
* **Framework**: ROS2 (Humble)
* **Programming**: Python
* **Computer Vision**: OpenCV
* **AI/ML**: Google Gemini 2.5 Flash, Google Speech Recognition API
* **Hardware**: Dobot Magician robotic arm (4-DOF with vacuum gripper)

## Technical Highlights

### Computer Vision Pipeline
- HSV-based color segmentation for robust block detection
- MinAreaRect for rotation estimation (full 360° with 0-90° normalization)
- Spatial proximity analysis for stack detection
- Real-time tracking with unique block identifiers

### LLM Integration & Spatial Reasoning
- Temperature parameter (0.1) for deterministic outputs
- Comprehensive scene context with distance matrices and spatial annotations
- Resolves ambiguous references ("nearest block", "farthest block", "between blocks")
- Stack protection intelligence prevents accidental structure disruption

### Motion Planning
- Persistent memory system maintains block positions across operations
- Dynamic Z-height calculation: Z_target = Z_base + n × h_block (11mm per block)
- Rotation matching for aligned placement
- Conservative collision avoidance with safe travel heights

## Results & Performance
- Successfully executed complex voice commands with multi-step reasoning
- Achieved millimeter-level positioning accuracy through homography transformation
- Zero collisions across extensive testing
- Seamless dual-mode operation (text and voice commands)
- End-to-end latency under 2 seconds for most operations

## Example Commands Executed
```
"Stack the red block on the blue block"
"Place the nearest block on the farthest one"
"Put green beside yellow on the right"
"Stack all blocks in order"
"Place blue between red and green"
```

## Impact
Created a system that bridges the gap between human intent and robot execution, allowing non-technical users to control complex robotic tasks through natural conversation—demonstrating the future of intuitive human-robot interaction.

**Project Duration**: November 2025 - December 2025  
**Course**: RAS 545 - Robotics and Autonomous Systems (Final Project)  
**Institution**: Arizona State University

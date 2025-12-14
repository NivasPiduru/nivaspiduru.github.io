---
title: "Autonomous Maze Solver Using Computer Vision and AI"
excerpt: "Robot that detects, plans, and navigates mazes of varying sizes using BFS algorithm and homography transformation"
collection: portfolio
---

## Project Links
* **GitHub Repository**: [View Code](https://github.com/NivasPiduru/autonomous-maze-solver-robot)
* **Video Demo**: [Watch Demo](https://youtu.be/uBfR9s_YYWY)

## Overview
Developed a fully autonomous robotic system capable of solving rectangular mazes of any size (3×3, 4×4, 5×5) without human intervention. The system integrates computer vision for maze detection, BFS path planning for optimal solutions, and precise robotic control with millimeter-level accuracy.

## Key Capabilities
* **Dynamic Maze Detection**: Automatically detects maze size without manual configuration
* **Optimal Path Planning**: BFS algorithm guarantees shortest path in 100% of cases
* **Precise Navigation**: <2mm positioning accuracy with homography-based coordinate transformation
* **Zero Collisions**: Perfect safety record across 20+ test runs

## Technical Stack
* **Framework**: ROS 2 (Humble) with modular three-node architecture
* **Computer Vision**: OpenCV - perspective correction, grid extraction, color-based marker detection
* **Algorithm**: Breadth-First Search (BFS) for guaranteed optimal paths
* **Coordinate Transformation**: Planar homography using DLT and SVD
* **Hardware**: Dobot Magician Lite robotic arm
* **Development**: AI-assisted development with Claude AI via ROS MCP Server (40% faster development)

## Results
- **95%** maze detection success rate
- **100%** optimal path finding (BFS guarantee)
- **±3mm** robot positioning accuracy
- **8-12 seconds** total solution time
- Successfully tested on 3×3, 4×4, and 5×5 mazes

**Project Duration**: November 2025  
**Course**: RAS 545 - Robotics and Autonomous Systems (Midterm 2)  
**Institution**: Arizona State University

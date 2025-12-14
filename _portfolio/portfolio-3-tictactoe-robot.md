---
title: "Autonomous Tic-Tac-Toe Playing Robot"
excerpt: "Interactive game-playing robot using computer vision and Minimax AI algorithm for intelligent opponent gameplay"
collection: portfolio
---

## Project Links
* **GitHub Repository**: [View Code](https://github.com/NivasPiduru/tictactoe-robot)
* **Video Demo**: [Watch Demo](https://youtube.com/shorts/eE9nDp7xyAE?feature=share)

## Overview
Created a fully automated Tic-Tac-Toe playing robot using the Dobot Magician Lite that plays against human opponents without intervention. The system uses computer vision to detect human moves, Minimax algorithm to calculate optimal counter-moves, and robotic control to physically place game pieces.

## Key Features
* **Computer Vision Detection**: Real-time game state analysis using OpenCV with HSV color detection
* **Minimax AI**: Perfect strategic gameplay - never loses, always wins or forces draw
* **Autonomous Operation**: Complete sense-think-act cycle without human intervention
* **Interactive Gameplay**: Player chooses color and turn order for customized experience
* **Error Prevention**: Color validation system prevents invalid moves

## Technical Implementation
* **Vision System**: HSV-based color segmentation for robust block detection, perspective warping for accurate board analysis
* **Game AI**: Minimax algorithm with recursive tree search, evaluates all possible move sequences, guarantees optimal play
* **Robot Control**: Pre-calibrated coordinate system for 9 grid cells and block pallets, suction cup end-effector for reliable pick-and-place
* **Hardware**: Dobot Magician Lite, USB camera (top-down view), colored blocks (red/blue)

## Bonus Features
* Player choice: Human or robot can go first
* Move validation: Detects and prevents color mismatches
* Turn-by-turn logging with game outcome announcement

## Results
- **100%** game completion rate without errors
- **Perfect AI performance** - never makes strategic mistakes
- **Reliable detection** under controlled lighting
- **Smooth gameplay** with consistent pick-and-place accuracy

**Project Duration**: October 2025  
**Course**: RAS 545 - Robotics and Autonomous Systems (Midterm 1)  
**Institution**: Arizona State University

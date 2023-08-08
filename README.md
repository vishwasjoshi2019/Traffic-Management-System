# Traffic-Management-System
"Smart Traffic Control System: Real-time Traffic Management using Image Processing and ML"
<p align="center">
 <img height=200px src="./traffic-signal.jpg" alt="Traffic Signal Timer">
</p>

<h1 align="center">Smart Traffic Signal Timer</h1>

<div align="center">

[![Python version](https://img.shields.io/badge/python-3.7-blue.svg)](https://www.python.org/downloads/release/python-370/)
[![License: Apache 2](https://img.shields.io/badge/License-Apache-yellow.svg)](https://www.apache.org/licenses/LICENSE-2.0)

<h4>This project introduces an innovative Smart Traffic Signal Timer that adapts to real-time traffic conditions using cameras, AI, and image processing. It aims to reduce congestion, speed up transit, and prioritize emergency vehicles.</h4>

</div>

-----------------------------------------

### Overview

Traffic congestion is a major issue in urban areas. This project presents a solution using AI and computer vision to manage traffic signals intelligently. The system analyzes live images from cameras at junctions to calculate traffic density and adjust signal timings accordingly, minimizing congestion and enhancing efficiency.

### Features

- **Real-time Traffic Density:** The system processes camera images to detect the density of vehicles, including cars, bikes, buses, and trucks.

- **Adaptive Signal Timing:** Based on traffic density, the system dynamically adjusts signal timings to alleviate congestion and improve traffic flow.

- **Emergency Vehicle Priority:** Emergency vehicles like ambulances receive special signal priority, reducing response times in critical situations.

### How It Works

The project consists of three modules:

1. **Vehicle Detection:** Uses YOLO object detection to count vehicles in camera images, determining traffic density.

2. **Signal Switching Algorithm:** Adjusts signal timings based on vehicle counts and other factors, optimizing traffic flow.

3. **Simulation Module:** A visual simulation showcases the system's effectiveness compared to static traffic control.

### Prerequisites

- Python 3.7
- Microsoft Visual C++ build tools (For Windows)

### Installation

1. Clone the repository: `git clone https://github.com/mihir-m-gandhi/Adaptive-Traffic-Signal-Timer`

2. Download the weights file [here](https://drive.google.com/file/d/1flTehMwmGg-PMEeQCsDS2VWRLGzV6Wdo/view?usp=sharing) and place it in `Adaptive-Traffic-Signal-Timer/Code/YOLO/darkflow/bin`.

3. Install required packages:
   ```sh
   cd Adaptive-Traffic-Signal-Timer/Code/YOLO/darkflow
   pip install -r requirements.txt
   python setup.py build_ext --inplace


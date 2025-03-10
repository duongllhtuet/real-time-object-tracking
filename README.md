# Real-Time Object Detection & Tracking for Autonomous Vehicles

## Overview
This project aims to develop a real-time object detection and tracking system for autonomous vehicles. The system processes video streams from vehicle-mounted cameras to detect and track objects such as pedestrians, vehicles, and traffic signs.

## Features
- **Real-time Object Detection**: Utilizes YOLOv8/EfficientDet for efficient detection.
- **Multi-Object Tracking**: Implements DeepSORT + OC-SORT for robust tracking.
- **High Performance**: Optimized with TensorRT and multi-threading for low latency.
- **Autonomous Vehicle Integration**: Works with CARLA simulator for testing in realistic environments.

## Project Structure
```
real-time-object-tracking/
├── docs/               # Documentation and research
├── src/                # Source code
│   ├── detection/      # Object detection models
│   ├── tracking/       # Object tracking modules
│   ├── integration/    # CARLA integration
├── models/             # Pretrained models and weights
├── data/               # Datasets and data preprocessing
├── scripts/            # Utility scripts for training and evaluation
├── experiments/        # Experiment results and benchmarks
├── results/            # Output videos and logs
├── Dockerfile          # Docker configuration
├── requirements.txt    # Dependency list
├── README.md           # Project overview and setup guide
├── LICENSE             # License information
└── .gitignore          # Files to be ignored by Git
```

## Installation
### Prerequisites
- Python 3.8+
- CUDA-enabled GPU (for acceleration)
- CARLA Simulator (for testing)

### Setup
```bash
git clone https://github.com/your-username/real-time-object-tracking.git
cd real-time-object-tracking
pip install -r requirements.txt
```

## Usage
### Running Object Detection & Tracking
```bash
python src/main.py --video input.mp4 --model yolo
```

### Running in CARLA Simulator
```bash
python src/integration/carla_tracking.py
```

## Results
Sample output from the tracking system:
![Demo](results/demo.gif)

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contribution
Feel free to fork this repository and submit pull requests for improvements.


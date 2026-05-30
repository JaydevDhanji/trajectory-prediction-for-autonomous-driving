# Real-time Graph-based Interaction-aware Trajectory Prediction for Autonomous Vehicles

## Project Overview

This repository contains the implementation and results of the thesis titled "Real-time Graph-based Interaction-aware Trajectory Prediction for Autonomous Vehicles." The project focuses on developing a system that predicts vehicle trajectories in real time using interaction-aware models based on graph representations.

## Project Structure

The repository is organized as follows:

```
├── data\_folder/
│   ├── first\_iteration/
│   │   ├── prediction\_test/
│   │   └── prediction\_train/
│   └── second\_iteration/
│       ├── prediction\_test/
│       └── prediction\_train/
├── data\_preparation/
│   ├── erase\_empty\_file.py
│   ├── extract\_data.py
│   ├── randomize\_data.py
│   └── split\_data.py
├── docs/
│   └── thesis.pdf
├── grip\_plus\_plus/
│   └── modified\_GRIP++/
├── metrics/
│   ├── calculate\_error\_metrics.py
│   └── identify\_epoch.py
├── results/
│   ├── numerical\_results/
│   └── videos/
├── visualize/
│   ├── overlay\_trajectory.py
│   └── segmentation\_and\_yolo.py
└── requirements.txt
```

## Installation

To set up the project environment, you will need Python 3 and pip. You can create a virtual environment (recommended) and install the required packages using the following commands:

```bash
# Create a virtual environment (optional)
python -m venv venv
source venv/bin/activate  # On Windows use: venv\\Scripts\\activate

# Install the required packages
pip install -r requirements.txt
```

## Usage

### Data Preparation

Before running the models, ensure that the data is correctly prepared. You can use the scripts in the `data\_preparation/` folder to clean and preprocess your data.

### Running the Model

1. Navigate to the folder containing the model scripts.
2. Run the desired script to start the training or testing process.

For example, to overlay trajectories, you can run:

```bash
python visualize/overlay\_trajectory.py
```

### Results

After running the models, you will find the output in the `results/` folder, including numerical results and generated videos.

## Contributing

If you would like to contribute to this project, please fork the repository and submit a pull request with your improvements or features.

## Original Code Links

For the foundational components of this project, you can refer to the original code repositories:

* [GRIP++](https://github.com/xincoder/GRIP) - This repository contains the original implementation of the GRIP++ framework.
* [JAAD Dataset](https://github.com/ykotseruba/JAAD) - This repository provides access to the JAAD dataset used for training and evaluating the models.


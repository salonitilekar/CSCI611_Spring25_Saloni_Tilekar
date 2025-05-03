# CSCI 611 – Spring 2025 – Assignment 2

**Name:** Saloni Tilekar

## 📚 Introduction

This repository contains **Assignment 2** for **CSCI 611**:

1. **Image Filtering** – Implemented various convolution-based filters.
2. **CNN for CIFAR-10 Classification** – Built, trained, and analyzed a convolutional neural network.

## 🚀 Getting Started

### Repository Structure

```
CSCI611_Spring25_Saloni_Tilekar/
└── Assignment_2/
    ├── image_filter.ipynb
    ├── build_cnn.ipynb
```

### Prerequisites

- Python 3.8+  
- Libraries: numpy, matplotlib, torch, torchvision, etc.  
- Jupyter Notebook or JupyterLab

### Installation

```bash
git clone https://github.com/<your-username>/CSCI611_Spring25_Saloni_Tilekar.git
cd CSCI611_Spring25_Saloni_Tilekar/Assignment_2
pip install numpy matplotlib torch torchvision jupyter
```

## 🛠️ Usage

1. **Image Filtering**  
   - Open `image_filter.ipynb` and run all cells.  
   - Implements filters: edge detection (horizontal, vertical), blurring (2×2, 3×3, 5×5).  
   - Outputs displayed inline within the notebook.

2. **CNN Model**  
   - Open `build_cnn.ipynb` and run all cells.  
   - Hyperparameters:
     - `batch_size = 32`  
     - `valid_size = 0.15`  
     - `lr (SGD) = 0.005`, `lr (Adam) = 0.0005`  
     - `num_workers = 2`  
     - `n_epochs = 15`  
   - Generates training/validation curves and final accuracy metrics.  
   - Training and validation plots are generated within the notebook.

3. **Report**  
   - Available as `report.pdf` (or embedded).  
   - Includes:
     - Architecture diagram  
     - Training curves  
     - Filter visualizations  
     - Key observations and findings

## 📊 Results & Observations

### Image Filtering

- **Edge Detection:** Custom weights reveal sharper diagonal edges compared to standard Sobel.  
- **Blurring:** Non-uniform 2×2 and larger kernels balance noise reduction with detail preservation.

### CNN Performance

| Optimizer | Accuracy |
|-----------|----------|
| SGD       | 73%      |
| Adam      | 65%      |

- **Architecture:** 4 convolutional layers (32 → 64 → 128 → 256 channels)  
- **Improvements:** Batch normalization, dropout (p=0.3), data augmentation (random flips, rotations)


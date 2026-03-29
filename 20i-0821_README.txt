CIFAR-10 Classification: ANN vs CNN vs Hybrid Model Comparison
=============================================================

Assignment: Deep Learning Assignment 2
Author: M Zain ul Abideen

OVERVIEW
--------
This project implements and compares three neural network architectures on CIFAR-10:
1. Ultra-Deep Residual ANN (Target: ≥65% accuracy)
2. Deep CNN (Target: ≥85% accuracy)  
3. Hybrid CNN+ANN (Target: ≥85% accuracy)

REPRODUCTION INSTRUCTIONS
-------------------------
1. Environment Setup:
   - Python 3.8+
   - PyTorch 1.9+
   - CUDA 11.0+ (for GPU acceleration)
   - Required packages: torch, torchvision, numpy, pandas, matplotlib, seaborn, scikit-learn

2. Install Dependencies:
   pip install torch torchvision numpy pandas matplotlib seaborn scikit-learn

3. Run the Notebook:
   - Open notebooks/cifar10_professional_comparison.ipynb
   - Run all cells in order from first to last
   - All outputs will be displayed within notebook cells
   - No external terminals required

4. Expected Runtime:
   - ANN Training: ~30-45 minutes (70 epochs)
   - CNN Training: ~25-35 minutes (50 epochs)
   - Hybrid Training: ~35-45 minutes (50 epochs)
   - Total: ~2-3 hours on GPU

REPRODUCIBILITY
---------------
- Random seed: 42 (set for numpy, torch, python)
- Deterministic operations enabled
- All hyperparameters documented in notebook
- Model checkpoints saved in checkpoints/ folder

TARGET ACCURACIES
-----------------
- Enhanced ANN: ≥75% (vs basic ANN ~65%)
- Deep CNN: ≥85% 
- Hybrid CNN+ANN: ≥85%

ARCHITECTURE HIGHLIGHTS
-----------------------
- ANN: Ultra-deep residual blocks, skip connections, GELU activation
- CNN: Residual conv blocks, global average pooling, batch normalization
- Hybrid: CNN feature extractor + deep ANN classifier

TRAINING FEATURES
-----------------
- Advanced data augmentation (crop, flip, color jitter, rotation, perspective)
- Label smoothing (0.1)
- AdamW optimizer with cosine annealing
- Gradient clipping (max_norm=1.0)
- Early stopping (patience=20)
- Learning rate scheduling

RESULTS
-------
The notebook will display:
- Training progress for each model
- Final test accuracies
- Model parameter counts
- Comprehensive comparison table
- Target achievement status

FILES STRUCTURE
---------------
20i-0821_Notebook.ipynb
checkpoints/
  └── [model checkpoints will be saved here]
20i-0821_README.txt
20i-0821_A2Report.pdf


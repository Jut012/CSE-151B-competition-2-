# Climate Change Model Competition

This repository contains the code, report, and final model used for the CSE 151B Climate Modeling Competition Project. The objective is to predict future surface temperature (`tas`) and precipitation (`pr`) fields from historical climate variables using deep learning.

##  Final Scores

- **Public Kaggle Score**: `1.14 RMSE`
- **Private Kaggle Score**: `1.35 RMSE`
- **Model Name**: `LatNorm–R–UNet` (Residual UNet with cosine normalization, hybrid loss, and pretrained encoder)

##  Contents

- `Final Climate Change Model.ipynb`: Final model notebook that achieved the best scores (1.14 / 1.35).
- `CSE_151B_Final_Report.pdf`: Full report including methodology, architecture diagrams, training details, results, and discussion.
- `CSE_151B_Competetion_Code.ipynb`: Earlier notebook used for initial experimentation and baseline model testing.
- `CSE_151B_Competetion_Code with dummy code.ipynb`: Additional notebook exploring a naive `DummyNet` baseline.
- `cse_151b_competetion_code.py`: Script version of the starter code.
- `final_climate_change_model.py`: Final version of the model (LatNorm-R-UNet)
- `CSE 151B Competition Milestone.pdf`: Initial milestone write-up (early model results and planning).
- `README.md`: This file.
- 
##  Models Overview

- **LatNorm–R–UNet (Final)**: Residual UNet with:
  - Cosine-weighted normalization
  - Huber + MSE hybrid loss
  - Log-transformed precipitation
  - ResNet-34 encoder with ImageNet pretraining

- **SimpleCNN-Res**: An intermediate baseline using residual blocks with smaller depth and no decoder.

- **DummyNet**: A naive $1\times1$ conv-only baseline with no spatial modeling.

##  How to Run

This repository is optimized for Google Colab. You can open `Final Climate Change Model.ipynb` in Colab and start training immediately.  
If running locally, use `final_climate_change_model.py` for script-based execution.

##  Notes

- Code uses PyTorch Lightning for training abstraction and reproducibility.
- Model checkpoints and logs can be configured to save during validation.
- Visual results and evaluation metrics are included in the final report.

##  Author

- Justin Tran — [jut012@ucsd.edu](mailto:jut012@ucsd.edu)


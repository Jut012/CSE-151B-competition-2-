# CSE-151B-competition-2-
This repository contains the code and report for the CSE 151B Climate Modeling Milestone Project. The objective is to predict future surface temperature (`tas`) and precipitation (`pr`) fields from historical climate variables using deep learning.

## Contents

- `CSE_151B_Competetion_Code.ipynb`: Main notebook used for experimentation and visualizations. Best viewed in Google Colab.
- `cse_151b_competetion_code.py`: Script version of the notebook for reproducibility or alternative execution (e.g., on a cluster or locally without Jupyter).
- `CSE 151B Competition Milestone.pdf`: Full milestone report including exploratory analysis, architecture breakdown, training setup, results, and reflections.
- `README.md`: This file.

## Models

- **DummyNet**: A naive baseline using a $1\times1$ convolution (no spatial context).
- **SimpleCNN-Res**: A residual CNN with progressively increasing depth and receptive field, designed to capture spatial dependencies and climate patterns.

## Instructions

This repository is designed to be run in [Google Colab](https://colab.research.google.com/). If using locally, you may run the `.py` script for training and evaluation.

## Notes

- The `.py` file mirrors the `.ipynb` notebook to ensure compatibility in non-notebook environments.
- Due to notebook rendering issues on GitHub, code review is easier using the script or Colab preview.

## Authors

- Justin Tran — [jut012@ucsd.edu](mailto:jut012@ucsd.edu)

## GitHub Access for Grading

TAs and Professor have been granted access under the following usernames:  
`salv47`, `nishant42491`, `atong28`, `AZA-2003`, `VedantMohann`, `charliespy`, `DivyamSengar`

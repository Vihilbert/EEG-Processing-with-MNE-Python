# ERP and Time-Frequency Analysis in Python using MNE

## Overview
This project focuses on analyzing EEG data using event-related potentials (ERP) and time-frequency analysis in Python with MNE. The workflow includes loading and processing trial-based EEG data, computing mean ERPs, and performing time-frequency analysis.

## Requirements
- Python 3.x
- Required libraries: `scipy`, `numpy`, `matplotlib`, `mne`
- EEG data in `.mat` and `.edf` formats
- Labels file (`Labels.txt`)

## Features
- **Trial-Based Data Analysis**: Load and extract EEG data from MATLAB files.
- **ERP Computation and Visualization**: Compute and plot mean ERPs for different conditions.
- **EEG Processing in MNE**:
  - Load and preprocess EEG data from EDF files.
  - Set up EEG montage.
  - Apply bandpass filtering.
  - Extract and epoch event-related data.
  - Compute and visualize ERPs for different conditions.
- **Time-Frequency Analysis**:
  - Perform Morlet wavelet transformation for time-frequency analysis.
  - Visualize time-frequency representations for a selected EEG channel.

## Usage
1. Load trial-based EEG data and inspect the structure.
2. Compute and visualize ERPs.
3. Import EEG data into MNE and preprocess it.
4. Epoch the EEG data based on event markers.
5. Compute and plot mean ERPs for different conditions.
6. Perform and visualize time-frequency analysis.

## Output
- ERP plots for different conditions.
- Time-frequency representations for selected EEG channels.

## Acknowledgments
This project utilizes MNE for EEG analysis and visualization. Ensure the required datasets (`Trial-based.mat`, `ERD_ERS.edf`, and `Labels.txt`) are available before running the scripts.


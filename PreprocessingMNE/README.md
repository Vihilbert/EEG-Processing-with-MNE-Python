Here’s a detailed README for your GitHub repository:

---

# **EEG Preprocessing with MNE**

This repository contains a Python script for processing and analyzing EEG (Electroencephalography) data using the **MNE** library. The script includes steps for reading, filtering, artifact removal, and visualization of EEG data.

## **Table of Contents**
- [Introduction](#introduction)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Steps of Processing](#steps-of-processing)
  - [Reading EEG Data](#reading-eeg-data)
  - [Plotting EEG](#plotting-eeg)
  - [Filtering EEG](#filtering-eeg)
  - [Removing Artifacts with ICA](#removing-artifacts-with-ica)
  - [Saving Processed Data](#saving-processed-data)
- [License](#license)

## **Introduction**
This script is designed to help process EEG data using the MNE library. It reads raw EEG data, applies filters to remove noise, removes artifacts using Independent Component Analysis (ICA), and plots the data at various stages of preprocessing. The final processed EEG data can be saved for further analysis.

## **Requirements**
To run this script, you will need the following Python libraries:
- `mne`: For EEG data processing
- `matplotlib`: For plotting EEG data

You can install the required libraries using pip:

```bash
pip install mne matplotlib
```

## **Installation**

1. Clone this repository:

```bash
git clone https://github.com/yourusername/EEG-Preprocessing.git
cd EEG-Preprocessing
```

2. Install the required dependencies:

```bash
pip install -r requirements.txt
```

## **Usage**

1. **Reading EEG Data**: 
   The script reads raw EEG data from an EDF file (using `mne.io.read_raw_edf`). Replace `'EDF_EEG.edf'` with the path to your own EEG data file.

2. **Plotting Raw EEG**: 
   The script visualizes the raw EEG data for a 10-second duration.

3. **Filtering EEG Data**: 
   The raw EEG is filtered between 0.1 and 30 Hz. You can adjust the frequency range depending on your needs.

4. **Removing Artifacts with ICA**: 
   Independent Component Analysis (ICA) is applied to remove artifacts from the EEG data. The ICA components are visualized and the artifact components can be excluded.

5. **Saving Processed Data**: 
   The script saves the filtered and artifact-free EEG data to a `.fif` file, which can be used for further analysis.

Run the script as follows:

```bash
python preprocess_eeg.py
```

Make sure to replace `'EDF_EEG.edf'` with the path to your raw EEG data file.

## **Steps of Processing**

### **Reading EEG Data**
```python
rawEEG = mne.io.read_raw_edf('EDF_EEG.edf', preload=True)
```
- This reads the raw EEG data from an EDF file into an MNE Raw object.

### **Plotting EEG**
```python
rawEEG.plot(block=False, duration=10.0, title='raw EEG data')
```
- Visualizes the raw EEG data for a 10-second window.

### **Filtering EEG**
```python
rawEEG.filter(0.1, 30)
```
- Filters the EEG data between 0.1 and 30 Hz to remove unwanted noise and artifacts.

### **Removing Artifacts with ICA**
```python
from mne.preprocessing import ICA
ICAComponents = ICA(15)
ICAComponents.fit(rawEEG)
```
- The script applies ICA with 15 components to remove artifacts from the EEG data.

### **Saving Processed Data**
```python
EEGFiltered.save('EEGFiltered.fif')
```
- Saves the filtered and artifact-free EEG data to a `.fif` file.

### **Plot After ICA Artifact Removal**
```python
rawEEG_ICA.plot()
```
- Visualizes the EEG data after ICA artifact removal.

## **License**

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---


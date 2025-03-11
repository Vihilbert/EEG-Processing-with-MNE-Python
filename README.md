---
---

# **EEG/ERP Analysis with Python and MNE**

This repository contains code for **EEG (Electroencephalography) and ERP (Event-Related Potentials) analysis** using Python and the **MNE-Python** library. EEG is a method used to measure electrical activity in the brain by placing electrodes on the scalp. ERPs are brain responses that are time-locked to specific sensory, cognitive, or motor events and are derived from EEG data.

The code in this repository covers fundamental EEG data preprocessing techniques, including filtering, artifact removal, and channel selection, as well as advanced steps for extracting and analyzing ERPs. The main focus is on applying time-frequency analysis and statistical methods to interpret EEG and ERP patterns for neuroscience and clinical research.

## **Table of Contents**
- [Introduction](#introduction)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Course Overview](#course-overview)
  - [EEG Data Preprocessing](#eeg-data-preprocessing)
  - [Event Detection and ERP Extraction](#event-detection-and-erp-extraction)
  - [Time-Frequency Analysis](#time-frequency-analysis)
- [License](#license)

## **Introduction**
EEG (Electroencephalography) is a non-invasive technique used to monitor the electrical activity of the brain. It involves recording voltage fluctuations resulting from ionic current flows within the neurons of the brain. EEG is widely used in both clinical settings for diagnosing conditions such as epilepsy and in research for studying brain activity during various tasks and cognitive states.

Event-Related Potentials (ERPs) are derived from EEG and reflect brain responses to specific external events or stimuli. Analyzing ERPs can provide insights into how the brain processes sensory inputs, cognitive functions, and responses to stimuli.

This repository contains Python code that demonstrates how to preprocess EEG data, remove artifacts, extract ERPs, and perform time-frequency analysis. It provides practical exercises and examples to help you get hands-on experience in EEG/ERP data analysis.

## **Requirements**
To run the code, you will need the following Python libraries:
- `mne`: For EEG data preprocessing and analysis
- `numpy`: For numerical operations
- `matplotlib`: For data visualization

You can install the required dependencies using pip:

```bash
pip install mne numpy matplotlib
```

## **Installation**

1. Clone the repository:

```bash
git clone https://github.com/yourusername/EEG-ERP-Analysis.git
cd EEG-ERP-Analysis
```

2. Install the required dependencies:

```bash
pip install -r requirements.txt
```

## **Usage**

1. **EEG Data Preprocessing**: 
   The scripts in this section demonstrate how to load, preprocess, and filter EEG data. You will learn how to remove artifacts using techniques such as Independent Component Analysis (ICA), and how to select relevant EEG channels for analysis.

2. **Event Detection and ERP Extraction**: 
   In this section, you will learn how to detect events in EEG data (such as visual or auditory stimuli) and how to extract ERPs that correspond to these events.

3. **Time-Frequency Analysis**: 
   Time-frequency analysis helps explore the frequency components of EEG signals over time. This section covers the application of time-frequency transformations to EEG data and visualization of power spectral density.

### **Example Usage**

To preprocess EEG data, simply run:

```bash
python preprocess_eeg.py
```

This script will:
1. Load raw EEG data.
2. Apply filtering and artifact removal.
3. Plot the preprocessed data.

For ERP extraction and time-frequency analysis, use the provided scripts like `extract_erp.py` and `time_frequency_analysis.py`.


## **License**

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

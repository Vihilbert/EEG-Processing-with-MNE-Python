
 
# EEG Preprocessing with MNE-Python

## Overview
This Jupyter Notebook performs preprocessing of EEG data using the MNE-Python library. The preprocessing steps include:
- Loading EEG data from a `.fif` file
- Applying a bandpass filter (1-40 Hz)
- Performing Independent Component Analysis (ICA) for artifact removal
- Visualizing raw, filtered, and cleaned signals

## Requirements
To run this notebook, install the following dependencies:
```bash
pip install mne numpy matplotlib
```

## Usage
1. **Set the file path**: Update the `file_path` variable with the path to your EEG data file.
2. **Define the time window**: Adjust `time_window` to select the portion of EEG data you want to analyze.
3. **Run the notebook**: Execute each cell to apply filtering, ICA, and visualization.

## Output
- **Raw EEG Signal**: Unprocessed EEG data visualization.
- **Filtered EEG Signal**: EEG signal filtered within the 1-40 Hz range.
- **Cleaned EEG Signal**: EEG signal after removing artifacts using ICA.

## Notes
- The ICA component exclusion is manually set (`ica.exclude = [0, 1]`). Adjust this based on your dataset.
- Ensure your `.fif` file is correctly formatted and accessible.

## License
This project is open-source and free to use.


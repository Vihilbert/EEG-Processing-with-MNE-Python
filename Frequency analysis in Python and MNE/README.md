---
---
# **Frequency Analysis of EEG Data in Python and MNE**

## **Overview**
This project demonstrates how to perform frequency analysis on EEG data using Python and MNE. The workflow includes loading EEG data, visualizing signals, applying Fast Fourier Transform (FFT), and computing power spectral density (PSD) using MNE's multitaper method. Additionally, it covers EEG topographical mapping for different frequency bands.

## **Workflow**
1. **Loading EEG Data**: EEG signals are imported from a text file (for single-channel data) and an EDF file (for multi-channel data) using MNE.
2. **Visualization**: EEG signals are plotted over time to inspect their amplitude variations.
3. **Frequency Analysis Using FFT**: The Fast Fourier Transform is applied to obtain the power spectrum, allowing analysis of dominant frequency components.
4. **Using MNE for Frequency Analysis**: EEG data is preprocessed with bandpass filtering, and PSD is computed for all channels.
5. **Topographical Mapping**: EEG activity across different scalp regions is visualized using topomaps for specific frequency bands (Theta, Alpha, Beta).

## **Tools & Libraries**
- **NumPy**: For numerical computations.
- **Matplotlib**: For visualizing EEG signals and frequency spectra.
- **MNE-Python**: For advanced EEG processing, PSD computation, and topographical mapping.




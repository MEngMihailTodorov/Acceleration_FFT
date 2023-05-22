# Acceleration_FFT
Unveil soil dynamics with this FFT Analysis tool. Decompose accelerometer data into unique frequencies, identifying soil vibration patterns and potential anomalies. Customize frequency range for focused insights. Ideal for engineers and data analysts.

FFT Analysis for Soil Response Spectra
This repository contains a Python-based Fast Fourier Transform (FFT) analysis procedure that is utilized to interpret accelerometer data, providing insights into soil dynamics. The scripts are designed to handle CSV files containing data recorded over time.

Overview
The key utility of this procedure is to transform raw, time-domain data into the frequency domain, allowing for the extraction of vital information from soil response spectra. It works by decomposing complex signals into individual sinusoidal components, revealing unique frequencies and their magnitudes that compose the overall signal. This provides a basis for understanding the soil response to various stimuli.

Procedure Steps
1. Data Preparation
Your data should be prepared in a CSV format, with the first column representing time and the second column representing acceleration.

2. Load Data
The CSV file is loaded into the script using pandas. Ensure the CSV file is correctly placed in the specified path.

3. Compute FFT
The FFT of the acceleration data is computed using the fft function from the scipy.fft module.

4. Compute Magnitude
The absolute values (magnitudes) of the FFT are computed. These values represent the strength of each frequency component in the signal.

5. Identify Frequencies
Frequency bins are computed to represent the frequencies present in the signal. These frequencies correspond to the calculated FFT magnitudes.

6. Plot FFT
The FFT magnitudes are plotted against their corresponding frequencies to visualize the frequency spectrum of the signal. Users can control the frequency range for analysis and visualization.

Additional Features
This procedure also helps users in identifying the fundamental frequency and the harmonic content of the soil vibration.

1. Fundamental Frequency
The frequency that corresponds to the maximum value in the FFT is the "natural frequency" or the fundamental frequency of the signal.

2. Harmonic Frequencies
Users can also find the second, third, and further harmonics based on the fundamental frequency.

This FFT Analysis for Soil Response Spectra is designed to facilitate the process of data interpretation, making it more accurate and insightful. It's a useful tool for geotechnical engineers, researchers, and data analysts.

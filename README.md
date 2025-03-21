# Noise Filtering of a Speech Signal

This project demonstrates various methods for filtering noise from a speech signal using Python. The goal is to isolate and reduce noise from audio recordings to improve the clarity and quality of the speech.

## Table of Contents

- [Introduction](#introduction)
- [Requirements](#requirements)
- [Usage](#usage)
- [Functions](#functions)
- [Examples](#examples)

## Introduction

Noise filtering is an essential process in audio processing, especially in applications involving speech recognition and communication systems. This project explores different techniques for normalizing signals, applying pre-emphasis filters, windowing with Hamming windows, and generating spectrograms.

## Requirements

To run the code in this project, you will need the following Python libraries:
- `numpy`
- `matplotlib`
- `scipy`
- `IPython`

You can install these dependencies using pip:

```bash
pip install numpy matplotlib scipy ipython
```
## Usage
To use the noise filtering functions, you can run the Jupyter Notebook file Noise filtering of a speech signal.ipynb. The notebook contains code cells that demonstrate the entire process from loading an audio file to filtering noise and visualizing the results.

## Functions
The project includes the following functions:

- normaliser(x): Normalizes a signal.
- preaccentuation(x): Applies a pre-emphasis filter to a signal.
- hamming(T): Generates a Hamming window.
- spectrogram(x, T, p, Tfft=None, pre=False, wind=None): Computes the amplitude and phase spectrogram of a signal.
- reconstituer(amp, phase, p): Reconstructs a signal from its amplitude and phase spectrogram.
- affich(S, fs, duree, log=True, maxfreq=None): Displays the amplitude spectrogram.
- energy(data, T, p): Calculates the energy of a signal.
- filtre_bandes(data, fs, minfreq, maxfreq, alpha): Applies a bandpass filter to a signal.
## Examples
The notebook provides examples of how to:

- Load and normalize an audio file.
- Compute and display the amplitude spectrogram.
- Filter noise using a bandpass filter.

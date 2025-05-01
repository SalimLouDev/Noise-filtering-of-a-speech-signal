This project focuses on filtering noise from speech signals to enhance audio clarity and quality using Python. Here's an expanded description of each section:

### Noise Filtering of a Speech Signal

This project explores various techniques for filtering noise from audio recordings, specifically targeting speech signals. The methods aim to improve speech clarity by isolating and reducing noise.

## Table of Contents

- [Introduction](#introduction)
- [Requirements](#requirements)
- [Usage](#usage)
- [Functions](#functions)
- [Examples](#examples)

## Introduction

Noise filtering in audio processing is crucial for applications such as speech recognition and communication systems. This project applies several processing techniques, including normalizing signals, using pre-emphasis filters, windowing with Hamming windows, and generating spectrograms to enhance speech signals.

## Requirements

To run this project, you'll need the following Python libraries:

- **`numpy`**: For numerical operations involving arrays.
- **`matplotlib`**: For plotting graphs and visualizing spectrograms.
- **`scipy`**: Provides functions for scientific and technical computing.
- **`IPython`**: Facilitates interactive computing, especially useful in Jupyter Notebooks.

Install the necessary libraries using pip:

```bash
pip install numpy matplotlib scipy ipython
```

## Usage

To explore the noise filtering techniques, execute the Jupyter Notebook named `Noise filtering of a speech signal.ipynb`. This notebook contains all necessary code, from loading an audio file to applying noise reduction techniques and visualizing the improved audio signal.

## Functions

This project comprises several key functions, each contributing to different stages of audio signal processing:

- **`normaliser(x)`**: Adjusts the amplitude of the signal `x` to a fixed range, ensuring consistency in signal processing.
- **`preaccentuation(x)`**: Applies a pre-emphasis filter to the signal, enhancing higher frequencies and improving speech intelligibility.
- **`hamming(T)`**: Generates a Hamming window of length `T`, reducing edge discontinuities in signals, aiding in subsequent spectral analysis.
- **`spectrogram(x, T, p, Tfft=None, pre=False, wind=None)`**: Computes and returns amplitude and phase spectrograms of a given signal `x`. These spectrograms provide a visual representation of the speech signal's frequency content over time.
- **`reconstituer(amp, phase, p)`**: Reconstructs a time-domain signal from its frequency-domain amplitude and phase spectrograms, facilitating verification of signal integrity following transformations.
- **`affich(S, fs, duree, log=True, maxfreq=None)`**: Plots the amplitude spectrogram `S` with frequency sampling `fs` over a specified duration `duree`. This visualization helps in analyzing the effectiveness of noise reduction techniques.
- **`energy(data, T, p)`**: Computes the energy of a signal across segments of length `T` using overlap `p`, providing insights into the intensity of different signal components.
- **`filtre_bandes(data, fs, minfreq, maxfreq, alpha)`**: Applies a bandpass filter to `data`, allowing only frequencies within `minfreq` to `maxfreq` to pass through, thereby reducing noise outside this frequency range.

## Examples

Refer to the Jupyter Notebook for hands-on examples demonstrating how to:

- Load an audio file and normalize its amplitude.
- Calculate and display the amplitude spectrogram, offering visual insights into frequency distribution over time.
- Apply a bandpass filter to isolate desired speech frequencies and diminish noise.

This expanded description gives a comprehensive overview of the project's purpose and methodology, clarifying its utility in noise reduction for speech signals.

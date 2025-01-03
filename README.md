# Real-Time Noise Cancellation System

## Overview

This project implements a real-time noise cancellation system designed to process live audio streams in two distinct scenarios:

1. **Single Speaker Scenario**: Isolates and enhances the primary speaker's voice while minimizing or eliminating interference from background noise and other voices.
2. **Multiple Speaker Scenario**: Preserves multiple speaker voices and filters out environmental noise (e.g., workplace noise, vehicle noise, etc.).

## Features

- **Real-Time Processing**: Processes audio in real-time with low latency (<100ms for each 200ms audio chunk).
- **Audio Input and Output**: Captures live audio input from a microphone and outputs a cleaned audio stream.
- **File Output**: Saves the processed, noise-reduced audio as a `.wav` file.
- **Pause/Resume**: Allows pausing and resuming of the audio stream during processing.

## Prerequisites

Ensure the following Python packages are installed before running the script:

- `pyaudio` - For audio stream handling.
- `numpy` - For data manipulation.
- `scipy` - For signal processing (e.g., filtering).
- `wave` - For saving the processed audio to a file.

```bash
pip install pyaudio numpy scipy keyboard
```

## Running the Script

1. Clone or download this repository.
2. Ensure the required dependencies are installed.
3. Run the script from the terminal or Python environment.
```bash
python noise_cancellation.py
```
4. The script will start recording and processing audio in real-time. It will save the cleaned audio to a .wav file and allow you to pause and resume the audio stream with a key press.


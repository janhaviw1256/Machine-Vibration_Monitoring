# Machine Vibration Monitoring Using FFT

## Project Overview

This project focuses on analyzing machine vibration signals using Digital Signal Processing (DSP) techniques, primarily FFT-based spectral analysis.

The objective is to identify important frequency components in vibration signals and use them to investigate possible bearing faults.

The project uses benchmark vibration data along with synthetic signals for validation and experimentation.

## Problem Statement

A machine is producing unusual vibrations.

Use FFT-based spectral analysis to determine the frequency components present in the vibration signal, identify dominant frequencies, and investigate whether the observed frequencies correspond to characteristic bearing fault frequencies.

## Dataset

The project uses benchmark bearing vibration data for analysis and validation.

Large raw datasets are not stored directly in this repository.

Dataset information and download instructions will be documented separately.

## Team Modules

### Member 1 — FFT and Spectrum Tools

- DFT implementation
- Radix-2 FFT implementation
- FFT validation
- Amplitude spectrum
- Synthetic signal generation
- FFT timing comparison
- Aliasing demonstration

### Member 2 — Data and Spectral Estimation

- Dataset loading
- Signal preprocessing
- Segmentation
- Windowing experiments
- Frequency-resolution experiments
- Welch spectral estimation

### Member 3 — Dominant Frequencies and Fault Diagnosis

- Peak detection
- Bearing geometry calculations
- Characteristic fault frequencies
- Theoretical vs measured frequency comparison
- Envelope analysis
- Fault-frequency interpretation

### Member 4 — Literature, Comparison and Report

- Literature review
- Related-work comparison
- Normal vs faulty comparison
- Report preparation
- Presentation support
- Final documentation

## Shared Configuration

Project-wide experimental parameters are stored in `config.py`.

Current shared parameters include:

- Sampling frequency: 12 kHz
- Short FFT size: 4096
- Long FFT size: 2¹⁵
- Default window: Hann
- Random seed: 42

## Testing

Unit tests will be maintained to validate the correctness of the implemented DSP methods.

The project will validate:

- Custom DFT against NumPy FFT
- Custom radix-2 FFT against NumPy FFT
- Parseval's theorem
- FFT linearity
- Synthetic frequency recovery
- Spectrum amplitude scaling
- Aliasing behavior

## Project Status

Currently in the repository setup and implementation stage.

The project will be developed incrementally, with each module validated before integration into the complete vibration-analysis pipeline.
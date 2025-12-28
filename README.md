# DriveWise - Driver Drowsiness Detection

**Author:** Mohini Pandey
**Publish Date:** December 28, 2025

## Table of Content
- [Overview](#overview)
- [Motivation](#motivation)
- [Technical Aspect](#technical-aspect)
- [Installation](#installation)
- [Run](#run)

## Overview
DriveWise is a real-time driver drowsiness detection system using live video feed from a camera. This project was developed to prevent accidents caused by drivers due to drowsiness; it will alert the driver when feeling sleepy by ringing an alarm. The CNN Model is used to identify whether the human eyes are closed or open with high accuracy. The Haar Cascade Classifiers are used for face, left eye, and right eye detection.

## Motivation
Currently, transport systems are an essential part of human activities. We all can be victims of drowsiness while driving, simply after a short night's sleep, altered physical condition, or during long journeys. This ultimately leads to dangerous situations and increases the probability of accidents. Driver drowsiness and fatigue are among the most critical causes of road accidents. Every year, they increase the number of deaths and fatal injuries globally.

## Technical Aspect
This project is divided into two parts:
1. Training a Convolutional Model to identify the human eye state.
2. Using Haar Cascade Classifiers and the trained model to detect drowsiness via edge deployment.

## Installation
The Code is written in Python. To install the required packages and libraries, run this command in the project directory:
```bash
pip install -r requirements.txt
```

## Run
- Run `DrowsinessModel.ipynb` which will train the CNN model and save it as `model.h5`.
- Move the trained model inside the `models` directory.
- Run `detection.py` which gets the live feed from your camera. The program analyzes the feed frame by frame using cascade models to detect human eyes, followed by the CNN model to classify the eyes. When the eyes are closed beyond a particular threshold, the alarm starts ringing.

## Contact
Developed by Mohini Pandey.

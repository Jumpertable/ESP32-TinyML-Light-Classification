# ESP32-TinyML-Light-Classification
An ESP32-based TinyML project using an LDR sensor
and Edge Impulse to classify lighting conditions.

## Project Overview

This project classifies light into three categories:

- Bright
- Normal
- Dark

## System Architecture

LDR Sensor → ESP32 → Data Collection →
Edge Impulse → INT8 Neural Network →
Real-Time Classification

## Hardware

- ESP32 Node32 Lite
- LDR Sensor
- Breadboard
- Jumper Wires
- USB Cable

## Model Architecture

| Layer | Configuration |
|---|---|
| Input | 5 Features |
| Hidden | 8 Neurons |
| Output | 3 Classes |

## Model Performance

| Metric | Result |
|---|---|
| Validation Accuracy | 82.9% |
| Testing Accuracy | 38.49% |
| Inference Time | Reported as 0 ms |
| RAM Usage | 1.2 KB |
| Flash Usage | 13.9 KB |

## Classification Results

The model successfully runs on the ESP32
and predicts Bright, Normal, and Dark.

Dark predictions reached over 90% confidence.
Bright and Normal predictions showed
greater uncertainty.

## Technologies

- Arduino IDE
- Edge Impulse
- C++
- TensorFlow Lite / EON Compiler
- INT8 Quantization

## Future Improvements

- Improve Bright and Normal classification
- Collect more balanced sensor data
- Improve dataset labeling
- Optimize the neural network


# Sign Language Detection

This repository contains a project for real-time sign language detection using computer vision and deep learning techniques. The goal is to recognize American Sign Language (ASL) gestures and convert them into text output.

## Features

- Real-time hand tracking using OpenCV and cvzone.
- Gesture recognition using a trained Keras model.
- Support for multiple sign language gestures.
- Easy-to-use interface for demonstration.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/ananya-s26/Sign-Language-Detection.git
   cd Sign-Language-Detection
   ```

2. Install the required libraries:
   ```bash
   pip install opencv-python numpy cvzone tensorflow
   ```

3. Ensure you have the Keras model and label files:
   - Place your trained Keras model (`keras_model.h5`) and labels (`labels.txt`) in the specified directories.

## Usage

1. Connect your webcam.
2. Run the detection script:
   ```bash
   python main.py
   ```
3. Use the following keys for interaction:
   - Press **'s'** to save the current gesture image.
   - Press **'q'** to quit the application.

## How It Works

1. **Hand Tracking**: The project uses the `cvzone` library to detect hands in real-time.
2. **Gesture Recognition**: The detected hand region is cropped and resized, then fed into a pre-trained Keras model to classify the gesture.
3. **Output Display**: The predicted gesture and its confidence level are displayed on the screen.

### Code Overview

- **Hand Detection**: Using OpenCV and the `HandDetector` class from `cvzone` to detect hands.
- **Gesture Classification**: Utilizing a Keras model to predict the gesture from the cropped hand image.
- **User Interface**: Displaying live video feed along with predictions.

## Contributing

Contributions are welcome! If you would like to contribute, please fork the repository and create a pull request. Make sure to update tests as appropriate.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

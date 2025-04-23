# NeuroScope

markdown
# NeuroScope: Real-Time Emotion Detection

NeuroScope is a real-time emotion detection system that uses deep learning and computer vision to identify human emotions from webcam footage. It uses a pre-trained CNN model for emotion classification and a DNN-based face detector for accurate face localization.

## Features
- Real-time face detection using OpenCV's DNN module
- Emotion classification using a pre-trained Keras model
- Audio feedback for detected emotions (optional)
- Customizable emotion labels, colors, and sound files

## Requirements
- Python 3.x
- Packages:
  - opencv-python
  - numpy
  - tensorflow
  - pygame

Install them using:

pip install opencv-python numpy tensorflow pygame
```

## Folder Structure
```
.
├── emotion_detection_model.h5           # Pre-trained emotion recognition model
├── deploy.prototxt                      # DNN model configuration file for face detection
├── res10_300x300_ssd_iter_140000.caffemodel # DNN model weights for face detection
├── sounds/                              # Folder containing audio files for emotions
│   ├── happy.wav
│   ├── sad.wav
│   ├── angry.wav
│   ├── surprise.wav
│   └── fear.wav
└── emotion_detector.py                  # Main Python script
```

## Usage
Run the script using:

```bash
python emotion_detector.py
```

- Press `q` to quit the webcam window.
- Make sure all model and sound files are in the correct paths.

## Customization
- Edit `EMOTION_LABELS` in the script to match your model's output classes.
- Update `SOUND_FILES` and `EMOTION_COLORS` dictionaries to change sound cues and bounding box colors.

## Notes
- Ensure your webcam is working and accessible.
- The default model input size is `(48, 48)`; update it if your model expects a different size.

## License
This project is open-source and free to use for educational and research purposes.
```

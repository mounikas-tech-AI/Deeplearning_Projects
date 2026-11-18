# Deeplearning_Projects
Real-Time Emotion and Emoji Recognition System

This notebook demonstrates a complete end-to-end pipeline to train a Convolutional Neural Network (CNN) to detect human emotions from grayscale facial images and map them to their corresponding emojis using OpenCV and Tkinter interfaces.

---

## 🛠️ Project Architecture
1. **Data Preparation**: Loading grayscaled face dataset (such as FER2013) from local directories using `ImageDataGenerator` with scaling normalization.
2. **Model Design**: Building a deep 2D Convolutional Neural Network using Keras Sequential API.
3. **Model Training**: Compiling and training the model on CPU/GPU, saving the weights locally as `emotion_model.h5`.
4. **Real-time Deployment**:
    * **Webcam feed**: Live OpenCV facial bounding boxes and emotion projection.
    * **Tkinter GUI Application**: Interactive display tracking human expressions with corresponding emojis.

---

## 🗂️ Setup and Requirements
Ensure you have the following folder structure for your scripts and assets:
```text
├── Documents/
│   └── Python Scripts/
│       ├── train/            # Train folder (7 classes of emotions)
│       └── test/             # Test/Val folder (7 classes of emotions)
└── emoji/
    ├── haarcascade_frontalface_default.xml
    ├── indianservers.jpg
    ├── angry.png
    ├── disgusted.png
    ├── fearful.png
    ├── happy.png
    ├── neutral.png
    ├── sad.png
    └── surpriced.png

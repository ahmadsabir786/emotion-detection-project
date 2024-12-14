# 🎭 Emotion Detection using OpenCV and MediaPipe

![Thumbnail](https://your-thumbnail-link-here.com)  


## 📖 Project Overview
This project leverages **OpenCV**, **MediaPipe**, and machine learning techniques to detect and classify human emotions from facial landmarks. The trained model identifies emotions such as:
- 😊 Happiness
- 😢 Sadness
- 😮 Surprise
- 😡 Anger
- 🤢 Disgust
- 😨 Fear
- 😐 Neutral

The application uses a webcam to capture real-time emotions and display predictions live! 🖥️

---

## 🚀 Features
- 🧠 **Facial Landmark Detection:** Powered by MediaPipe Face Mesh.
- 📊 **Emotion Classification:** Employs a Random Forest Classifier to detect emotions.
- 🎥 **Real-time Prediction:** Detect emotions via webcam in real-time.
- 📁 **Dataset Handling:** Reads images from a structured dataset, extracts landmarks, and labels them for training.

---

## 🛠️ Tech Stack
- **Programming Language:** Python 🐍
- **Libraries:**
  - OpenCV
  - MediaPipe
  - NumPy
  - scikit-learn
  - Pickle

---

## 📂 Project Structure
```
Emotion-Detection/
│
├── utils.py           # Helper functions (e.g., `get_face_landmarks`)
├── train_model.py     # Training script for the emotion classifier
├── predict.py         # Real-time emotion prediction script
├── data/              # Dataset directory
├── data.txt           # Preprocessed dataset
├── model.h3           # Trained Random Forest model
└── README.md          # Project documentation
```

---



---

## 📋 Installation
1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/emotion-detection.git
   ```
2. Navigate to the project directory:
   ```bash
   cd emotion-detection
   ```
3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

---

## 🧑‍💻 Usage
### 1. Prepare the Dataset
Place your labeled images in the `data/` directory with the following structure:
```
data/
├── HAPPINESS/
├── SADNESS/
├── SURPRISED/
├── ANGER/
├── DISGUST/
├── FEAR/
└── NEUTRAL/
```

### 2. Train the Model
Run the training script to train the emotion classifier:
```bash
python train_model.py
```

### 3. Real-Time Emotion Detection
Run the prediction script to use your webcam for real-time emotion detection:
```bash
python predict.py
```

---

## 🔍 How It Works
1. **Facial Landmarks Extraction:**
   - Detects 468 landmarks on a face using MediaPipe Face Mesh.
   - Normalizes and processes these landmarks as features for training.

2. **Model Training:**
   - Uses Random Forest Classifier for emotion recognition.
   - Achieves high accuracy using labeled facial landmark data.

3. **Real-Time Prediction:**
   - Captures video from the webcam.
   - Processes each frame for landmarks and predicts emotions live.

---

  ```
  [Add your confusion matrix output here]
  ```

---


---

## 🤝 Contributing
Contributions are welcome! If you'd like to make this project better, feel free to fork the repository and submit a pull request. 

---


## 🙌 Acknowledgments
- MediaPipe for the Face Mesh solution.
- OpenCV for robust computer vision functionalities.
- scikit-learn for powerful machine learning tools.

---

### 🌟 Don't forget to give this project a ⭐ on [GitHub](https://github.com/your-username/emotion-detection)! 😊

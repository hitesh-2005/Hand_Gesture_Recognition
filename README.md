# PRODIGY_ML_04
# ✋🖐️ Task 4 – Hand Gesture Recognition | Machine Learning Internship @ Prodigy Infotech

This project aims to develop a model that can classify different **hand gestures** using near-infrared images captured via the **Leap Motion Controller**. This task demonstrates practical applications of computer vision in human-computer interaction.

---

## 📁 Dataset Overview

- **Source:** Leap Motion infrared imagery
- **Gestures:** 10 distinct hand gestures (e.g., palm, fist, L, down)
- **Subjects:** 10 individuals (5 males, 5 females)
- **Images:** Each gesture has several sample frames captured from both hands

---

## 🗂️ Folder Structure

LeapGestureDataset/
├── 00/
│ ├── 01_palm/
│ │ ├── frame_XXXXX_l.png
│ │ └── frame_XXXXX_r.png
│ ├── 02_l/
│ └── ...
├── 01/
├── ...
├── 09/

yaml
Copy
Edit

- `00`, `01`, ..., `09`: Folder for each subject
- Inside each subject folder: gesture-specific directories
- Each gesture folder contains left and right hand infrared frames

---

## 📦 Project Structure

PRODIGY_ML_04/
├── Prodigy04.ipynb # Main Jupyter notebook for preprocessing, training, and evaluation
├── LeapGestureDataset/ # Dataset folders as described above
├── model/ # (Optional) Saved models or checkpoints
└── README.md # Project documentation

yaml
Copy
Edit

---

## 🛠️ Requirements

- Python 3.8+
- TensorFlow / PyTorch
- OpenCV
- NumPy
- matplotlib
- scikit-learn
- pandas
- tqdm

---

## 🚀 How to Run

1. **Download and unzip** the dataset into the `LeapGestureDataset/` directory.
2. **Open** the `Prodigy04.ipynb` notebook.
3. **Follow the steps** to:
   - Load and preprocess images (resize, grayscale conversion, etc.)
   - Encode gesture labels
   - Train a CNN model on gesture classification
   - Evaluate performance and visualize results

---

## 📊 Model Summary

- **Architecture:** Convolutional Neural Network (CNN)
- **Input:** Grayscale images (preprocessed)
- **Output:** Multiclass classification (0–9) for each gesture
- **Loss Function:** Categorical Cross-Entropy
- **Optimizer:** Adam

---

## 💡 Key Highlights

- Hand gesture recognition using real infrared sensor data
- Demonstrates image classification beyond visible spectrum
- Useful for applications in:
  - Sign language translation
  - Gesture-based UIs
  - VR/AR interactions

---

## 🔬 Limitations & Improvements

- **Grayscale input** limits information vs. RGB; future enhancement could explore depth data
- **Augmentation** (flipping, rotation) could improve generalization
- **Transfer learning** may boost performance with limited data

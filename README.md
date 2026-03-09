# 📝 Hand-Written Digit Recognition with CNN (MNIST)

This project implements a **Convolutional Neural Network (CNN)** using TensorFlow/Keras to recognize hand-written digits from the MNIST dataset. It features an interactive OpenCV-based GUI that allows users to draw digits with their mouse and get real-time predictions.

## 🚀 Key Features

* **Automated Training:** Loads the MNIST dataset and trains a high-accuracy CNN model.
* **Interactive Drawing Canvas:** A 400x400 black canvas for user input via mouse.
* **Real-time Prediction:** Pre-processes the drawing (resizing to 28x28 and normalization) to match the model's input requirements.
* **Overfit Protection:** Uses **Dropout** layers to ensure the model generalizes well to new, hand-drawn data.

---

## 🛠️ Tech Stack

* **Python 3.x**
* **TensorFlow / Keras** (Deep Learning Framework)
* **OpenCV** (Image Processing & UI)
* **NumPy** (Numerical Computing)

---

## 📸 Project Demo

Below you can see the model in action, predicting digits drawn on the canvas:

![Digit Recognition CNN](https://github.com/user-attachments/assets/e3f45f78-2b25-4e95-9e79-7e43ecda9709)
<img width="1345" height="1233" alt="image" src="https://github.com/user-attachments/assets/46ed5e62-7891-4c55-9f97-1d1a88d4db51" />



---

## ⚙️ Installation & Usage

1. **Clone the repository:**
```bash
git clone https://github.com/your-username/digit-recognition-cnn.git
cd digit-recognition-cnn

```


2. **Install dependencies:**
```bash
pip install tensorflow opencv-python numpy

```


3. **Run the script:**
```bash
python main.py

```



---

## 🎮 How to Use the Interface

Once the "Dibuja un digito" window opens, use the following keyboard shortcuts:

| Key | Action |
| --- | --- |
| **`p`** | **Predict:** Processes the current drawing and displays the result (digit + confidence %). |
| **`c`** | **Clear:** Wipes the canvas clean for a new drawing. |
| **`q`** | **Quit:** Safely closes the application. |

---

## 🧠 Model Architecture

The CNN follows a structured approach to feature extraction:

1. **Conv2D (32 filters, 3x3)** + MaxPooling: Detects basic edges and curves.
2. **Conv2D (64 filters, 3x3)** + MaxPooling: Extracts more complex shapes.
3. **Flatten:** Converts 2D feature maps into a 1D vector.
4. **Dropout (0.5):** Prevents the model from memorizing training data.
5. **Dense (128 units):** Fully connected layer with ReLU activation.
6. **Softmax (10 units):** Final output layer for classification (digits 0-9).

---

## ✒️ Author

* **Francisco Rivera** - [GitHub Profile](https://github.com/francisco-rivera-viveros)

---

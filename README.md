---

## 🌿 About

This project implements a **non-destructive plant nutrient assessment system** using **image processing and deep learning techniques** to classify plant health based on nutrient availability. The primary focus is detecting **nitrogen deficiencies** in maize plants by analyzing leaf images—without causing any damage to the plant.

By leveraging **spectral features and visual cues**, this system enables early and accurate diagnosis of nutrient stress, helping farmers make informed decisions in real time.

---

## 🧪 Application Overview

* **Objective**: Identify nutrient stress levels (e.g., N0, N75, Healthy) in maize plants using leaf imagery.
* **Methodology**: Image classification using a convolutional neural network (CNN) trained on a custom dataset.
* **Use Case**: Early-stage nutrient diagnosis for **precision agriculture** to enhance yield and reduce unnecessary fertilizer use.

---

## 📂 Dataset

* **Classes**:

  * `N0`: Nitrogen-deficient
  * `N75`: Moderately nitrogen-fed
  * `Healthy`: Optimal nitrogen supply

* **Directory Structure**:

  ```
  /Maize/Images/
  ├── N0/
  ├── N75/
  └── Healthy/
  ```

* **Image Type**: RGB images captured under natural lighting

* **Preprocessing**: Resizing, normalization, and augmentation (rotation, flipping, etc.)

---

## 🧠 Model Architecture

* **Framework**: PyTorch (v2.4.1)
* **Base Model**: Custom CNN / ResNet-based architecture (customizable)
* **Layers**: Convolutional, ReLU, MaxPooling, Fully Connected
* **Loss Function**: Cross-Entropy Loss
* **Optimizer**: Adam / SGD
* **Metrics**: Accuracy, Precision, Recall, F1-score

---

## 🚀 How to Run

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/non-destructive-plant-nutrient-assessment.git
   cd non-destructive-plant-nutrient-assessment
   ```

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Prepare the dataset:

   * Place your image folders (`N0`, `N75`, `Healthy`) inside `/Maize/Images/`

4. Train the model:

   ```bash
   python train.py
   ```

5. Evaluate / Predict:

   ```bash
   python evaluate.py
   python predict.py --image path/to/image.jpg
   ```

---

## 📈 Results & Outputs

* **Confusion Matrix**
* **Training Accuracy vs Epoch**
* **Loss Curve**
* **Sample Prediction Visuals**

> Optionally, you can integrate the model into a **GUI** or **web app** for field usability.

---

## 🧾 License

This project is licensed under the MIT License — see the `LICENSE` file for details.

---

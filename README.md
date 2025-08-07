# 🌪️ Cyclone Intensity Prediction Using INSAT-3D Satellite Imagery

This project implements a hybrid deep learning model using a custom CNN and a modified AlexNet to predict the intensity of tropical cyclones using half-hourly IR imagery from the INSAT-3D satellite.

## 📌 Features
- Real-time cyclone intensity prediction
- Trained on 40+ Indian Ocean cyclones (2014–2023)
- Custom CNN for spatial feature extraction
- Modified AlexNet for temporal intensity learning
- Automated preprocessing pipeline
- Low error: MAE = 0.0049, RMSE = 0.0049

## 🧠 Model Architecture
A hybrid of:
- 🧩 Custom CNN
- 🧩 Modified AlexNet
- Fusion via weighted averaging of outputs

## 🗂️ Folder Structure

/data - Sample IR images
/notebooks - Jupyter notebooks for training
/src - Model definitions and training logic
/utils - Preprocessing and visualization helpers
## 🚀 How to Run
1. **Clone the repo**:
git clone https://github.com/Shreyrath0re/cyclone-intensity-prediction-INSAT3D.git
cd cyclone-intensity-prediction-INSAT3D

2. **Install dependencies**:
pip install -r requirements.txt

3. **Train the model**:
python main.py

4. **Run inference**:
python src/inference.py --image path/to/image.png

🧪 Requirements
Python 3.8+
TensorFlow / PyTorch (whichever you used)
OpenCV, NumPy, Matplotlib, etc.
(Full list in requirements.txt)

**EVALUATION**:
| Model            | MSE        | RMSE      | MAE       |
| ---------------- | ---------- | --------- | --------- |
| Custom CNN       | 297.78     | 17.26     | 16.72     |
| Modified AlexNet | 338.69     | 18.40     | 18.00     |
| **Hybrid Model** | **254.79** | **15.96** | **15.30** |

This project is licensed under the MIT License - see the LICENSE file for details.

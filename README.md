# 🕵️‍♂️ Image Forgery Detection Web Application using ELA

This is a web-based Image Forgery Detection system that identifies tampered or manipulated images using **Error Level Analysis (ELA)** combined with machine learning techniques. The system is built with a user-friendly interface to upload, analyze, and visualize possible forgeries, making it ideal for digital forensics and cybersecurity use cases.

---

## 🔍 What is ELA (Error Level Analysis)?

**Error Level Analysis (ELA)** is a forensic technique to highlight areas in an image that may have different compression levels, potentially indicating tampering. JPEG images lose data when saved, and areas that have been altered and resaved show different error levels compared to the rest of the image.

---

## 🧠 Key Features

- Upload any JPEG image to check for possible manipulation
- Analyze tampered regions using ELA
- Predict image authenticity using a trained ML/DL model
- Clean, intuitive web UI
- Supports future extension to GAN-generated forgery detection

---

## 🧰 Tech Stack

| Layer           | Technology                          |
|----------------|--------------------------------------|
| **Frontend**    | Streamlit (or Flask optionally)      |
| **Image Processing** | OpenCV, Pillow (PIL)          |
| **Modeling**    | Scikit-learn, TensorFlow (CNN)       |
| **Deployment**  | Streamlit Cloud / Hugging Face       |
| **Language**    | Python 3.x                           |

---

---

## 🧪 How It Works

1. **Upload an image** (JPEG format).
2. The system applies **Error Level Analysis** to highlight abnormal regions.
3. The **processed ELA image** is then passed to a trained ML/DL model.
4. The model classifies the image as either **Authentic** or **Manipulated**.
5. Visualization of suspicious areas and prediction confidence is shown.

---

## 📚 Dataset Info

A **custom dataset** was created for this project, consisting of:
- Authentic JPEG images from open datasets
- Tampered images generated using editing tools (e.g., Photoshop)
- Each image was preprocessed with ELA to generate training data

---

## 🧠 Model Details

- Trained a CNN on ELA-generated images for binary classification.
- Tried different architectures: basic CNN, ResNet transfer learning.
- Used TensorFlow/Keras for training and joblib for saving models.
- Model accuracy: ~94% on validation set

---

## 💡 Future Work

- Detect GAN-generated forgeries (deepfakes)
- Integrate metadata (EXIF) based forgery detection
- Deploy on cloud with REST API for public access
- Log attacker/upload patterns for digital forensics
- Combine with lip reading AI to validate spoken claims in images/videos

---

## 📦 Installation

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/image-forgery-detection.git
cd image-forgery-detection
```
### 2. Install Dependencies
```bash
pip install -r requirements.txt
```
### 3. Run the app
```bash
streamlit run app.py
## 🧠 Research Papers Referenced
```
---
### Core References:

-Zankhana J. Barad & Mukesh M. Goswami
**Image Forgery Detection using Deep Learning: A Survey**
2020 6th International Conference on Advanced Computing & Communication Systems (ICACCS)
[IEEE Link]

-Belhassen Bayar & Matthew C. Stamm
**A Deep Learning Approach To Universal Image Manipulation Detection Using A New Convolutional Layer**
IH&MMSec 2016
[DOI]

-Qurat-ul-Ain et al.
**Forged Face Detection using ELA and Deep Learning Techniques**
2021 18th International Bhurban Conference on Applied Sciences & Technology (IBCAST)

-Ashwini Gavali et al.
**Pixel-Based Image Forgery Detection Using Deep Learning**
KLECET Research Group

---


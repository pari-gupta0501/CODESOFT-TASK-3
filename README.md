# CODESOFT-TASK-3

---

# 📸 Image Captioning using Deep Learning

## 🧠 Project Objective

To build an AI model that automatically generates descriptive captions for input images using a combination of CNN (InceptionV3) and RNN (LSTM) architectures.

---

## 🚀 Technologies Used

Python

TensorFlow / Keras

NumPy, Matplotlib

Pre-trained InceptionV3 (for feature extraction)

LSTM (for sequence modeling)

---

## 📁 Dataset

You can use:

Flickr8k or Flickr30k

OR a custom dataset with image_path -> captions format

---

## 🔧 How It Works

Feature Extraction: Images are processed using InceptionV3 to extract deep features.

Text Preprocessing: Captions are cleaned, tokenized, and padded.

Model Training: LSTM is trained on image features + captions.

Caption Generation: New captions are generated using a greedy approach.

---

## 🛠️ File Structure

image-captioning/

├── images/              # Image dataset

├── captions.txt         # Captions for each image

├── model.py             # CNN + RNN model

├── train.py             # Model training code

├── app.py               # Caption generation script

├── utils.py             # Helper functions

└── README.md            # Project documentation

---

## ✅ Steps to Run

1. Install Dependencies
```
pip install tensorflow keras numpy matplotlib pillow
```
2. Extract Image Features
```
### Inside utils.py

features = extract_features('images/example.jpg')
```
3. Clean Captions and Tokenize
```
cleaned = clean_caption("A boy playing with a dog")
```
4. Train Model
```
python train.py
```
5. Generate Caption
```
python app.py

### Output: "A boy is playing with a ball"
```
---

## SAMPLE OUTPUT

<img width="468" height="414" alt="image" src="https://github.com/user-attachments/assets/18322aed-6725-4215-b680-7c2c9764aaa6" />


## 📌 Future Improvements

Use Beam Search instead of Greedy Search

Use Attention Mechanisms

Deploy as a Web App

---

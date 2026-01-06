# ✈️ Aircraft Damage: Classification & Captioning 📸
## 📌 Overview
This comprehensive Deep Learning project automates the inspection of aircraft surfaces. It not only classifies structural damage (dents vs. cracks) using Computer Vision but also generates natural language descriptions of the damage using Generative AI. The system combines a VGG16 classifier with the BLIP (Bootstrapping Language-Image Pre-training) model to provide both categorical labels and detailed textual summaries.

## 🚀 Key Features

### 🔍 Damage Classification:
Uses a pre-trained VGG16 model (Transfer Learning) to accurately classify images as dent or crack.

### 📝 Automated Captioning:
Integrates the Salesforce BLIP model to generate human-readable captions and summaries of the damage (e.g., "This is a detailed photo showing a dent on the fuselage").

### 🔄 Hybrid Framework: 
Demonstrates advanced interoperability by wrapping a PyTorch Hugging Face model within a custom TensorFlow/Keras layer (BlipCaptionSummaryLayer).

### 🖼️ End-to-End Pipeline:
Automated dataset downloading, image preprocessing (rescaling/augmentation), training, evaluation, and inference.

### 📊 Visual Analytics: 
Includes tools for visualizing training metrics (Loss/Accuracy) and displaying prediction grids with Ground Truth vs. Predicted labels.

### 🛠️ Technologies Used
#### Deep Learning:
                  🧠 TensorFlow, Keras, PyTorch

#### Generative AI: 
                  🤗 Hugging Face Transformers (BLIP Model)

#### Computer Vision:
                  👁️ VGG16 (ImageNet weights), OpenCV/PIL

#### Data Handling:
                  🐼 NumPy, Pandas, Zipfile/Tarfile

#### Visualization: 
                  📉 Matplotlib

## 📂 Dataset
The system utilizes the Aircraft Damage Dataset, automatically downloaded and split into:

Training/Validation: For optimizing the VGG16 classifier.

Testing: For evaluating classification accuracy and generating caption inferences.

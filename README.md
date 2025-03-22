# Attention U-Net for Retinal Blood Vessel Segmentation

This repository contains the PyTorch implementation of **Attention U-Net** applied to the **DRIVE dataset** for blood vessel segmentation in retinal images. The model is based on the paper:

> Oktay et al., "Attention U-Net: Learning Where to Look for the Pancreas," [arXiv:1804.03999](https://arxiv.org/pdf/1804.03999.pdf).

The implementation is inspired by the **Towards Data Science** tutorial by **Hong Jing**, which provides a detailed step-by-step guide for biomedical image segmentation using Attention U-Net.

## 📌 **Project Overview**
Retinal blood vessel segmentation is crucial for the diagnosis and treatment of various cardiovascular and ophthalmologic diseases, including:
- **Diabetic Retinopathy**
- **Hypertension**
- **Arteriosclerosis**
- **Choroidal Neovascularization**

The DRIVE dataset is widely used for comparative studies in retinal vessel segmentation and morphological analysis of retinal blood vessels.

### **Why Attention U-Net?**
The **Attention U-Net** architecture improves standard U-Net by introducing attention gates, which help the model focus on relevant regions in the image, leading to:
- **Better segmentation accuracy**
- **Reduced false positives**
- **Improved focus on small vessels**

## 🏗 **Project Structure**
```
├── data/                # Dataset (DRIVE images & masks)
├── models/              # Model implementation (Attention U-Net)
├── notebooks/           # Jupyter Notebooks for training & visualization
├── utils/               # Helper functions
├── train.py             # Training script
├── test.py              # Evaluation script
├── requirements.txt     # Dependencies
└── README.md            # Project documentation
```

## 🚀 **Installation & Setup**
### **1. Clone the Repository**
```sh
git clone https://github.com/yourusername/attention-unet-drive.git
cd attention-unet-drive
```

### **2. Install Dependencies**
```sh
pip install -r requirements.txt
```

### **3. Download the DRIVE Dataset**
The dataset can be downloaded from [DRIVE Database](https://drive.grand-challenge.org/) and should be placed inside the `data/` directory.

### **4. Train the Model**
```sh
python train.py --epochs 100 --batch_size 4 --lr 0.001
```

### **5. Evaluate the Model**
```sh
python test.py
```

## 📊 **Results & Visualizations**
The model produces accurate segmentation of blood vessels. Sample results:

| Input Image | Ground Truth | Prediction |
|------------|--------------|-----------|
| ![Input](examples/input.png) | ![GT](examples/ground_truth.png) | ![Pred](examples/prediction.png) |

## 🔬 **Key Features**
✅ **Attention Mechanism**: Focuses on important regions in the image.
✅ **Dice Loss & Focal Loss**: Handles class imbalance effectively.
✅ **Data Augmentation**: Improves model generalization.
✅ **PyTorch Dataset Class**: Efficient data loading & preprocessing.

## 🔗 **References**
- **[Attention U-Net Paper](https://arxiv.org/pdf/1804.03999.pdf)**
- **[DRIVE Dataset](https://drive.grand-challenge.org/)**
- **[Hong Jing's Tutorial](https://towardsdatascience.com/biomedical-image-segmentation-attention-u-net-29b6f0827405)**

## 👨‍💻 **Contributors**
- **Your Name** ([@yourusername](https://github.com/yourusername))

---
Feel free to contribute by submitting pull requests or opening issues! 🚀



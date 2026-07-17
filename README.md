# 🐶🐱 Image Classification using Transfer Learning

## 📖 Notebook

The complete implementation is available here:

`notebooks/Image_Classification_Transfer_Learning.ipynb`

## 📌 Overview

This project implements image classification using **Transfer Learning** with a pretrained **ResNet18** model on the **Oxford-IIIT Pet Dataset**.

Two transfer learning approaches were implemented and compared:

- Feature Extraction
- Fine-Tuning

The performance of both methods was evaluated using accuracy, classification report, and confusion matrix.

---

## 📂 Dataset

- Oxford-IIIT Pet Dataset
- 37 Cat and Dog Breeds
- RGB Images

---

## 🧠 Model

- ResNet18 (Pretrained on ImageNet)

---

## ⚙️ Transfer Learning Methods

### Feature Extraction

- Frozen pretrained backbone
- Trained only the final classification layer

### Fine-Tuning

- Unfroze Layer4 and the final classification layer
- Fine-tuned using a smaller learning rate

---

## 📊 Results

| Method | Train Accuracy | Test Accuracy |
|---------|---------------:|--------------:|
| Feature Extraction | **91.93%** | **86.05%** |
| Fine-Tuning | **99.54%** | **88.55%** |

Fine-Tuning achieved better performance by allowing the last residual block to adapt to the new dataset.

---

## 📁 Project Structure

```
Image-Classification-Transfer-Learning/
│
├── notebooks/
│   └── Image_Classification_Transfer_Learning.ipynb
│
├── models/
│   ├── resnet18_feature_extraction.pth
│   └── resnet18_finetuned.pth
│
├── README.md
├── requirements.txt
└── .gitignore
```

---

## 🛠️ Technologies Used

- Python
- PyTorch
- Torchvision
- NumPy
- Matplotlib
- Scikit-learn

---

## 🚀 Future Improvements

- Train for more epochs
- Try deeper pretrained models (ResNet50, EfficientNet)
- Hyperparameter tuning
- Better data augmentation

---

## 👨‍💻 Author

**Arsh**


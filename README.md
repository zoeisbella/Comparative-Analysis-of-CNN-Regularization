# 🧠 Comparative Analysis of CNN Regularization Techniques

> 🔍 A Visual Experiment on How Data Augmentation, Group Normalization & Dropout Affect Model Performance

## 📖 Project Background

In deep learning image classification tasks:
- 🎨 **Data Augmentation** expands training data diversity
- 🛑 **Dropout** helps mitigate overfitting risks  
- ⚖️ **Group Normalization** stabilizes the training process

This project designs **8 controlled experiments** 🧪 to quantitatively analyze how these techniques perform individually and in combination, providing practical insights for model optimization in similar tasks! 📊

## 🛠 Tech Stack

| Component | Technology |
|-----------|------------|
| 🧩 **Deep Learning Framework** | TensorFlow 2.x + Keras |
| 🗂 **Dataset** | CIFAR-10 (10 classes of 32×32 color images) |
| 📈 **Visualization Tool** | Matplotlib |
| 💻 **Runtime Environment** | Python 3.7+, Jupyter Notebook (or any Python IDE) |

## 🧪 Experimental Design

We designed **8 technical combinations** covering four dimensions:

| Dimension | Description | 
|-----------|-------------|
| 🔰 **Baseline Model** | Plain CNN without regularization |
| ⚡ **Single Technique** | One regularization method at a time |
| 🤝 **Dual-Technique Combination** | Pairwise combinations |
| 🎯 **Triple-Technique Combination** | All three techniques together |

## 📊 Experimental Results
## 📊 Experimental Results

### 1. 📈 Accuracy Curve Comparison

**Left**: Training Accuracy Curve - The model's "practice" performance on the training set 🏋️  
**Right**: Validation Accuracy Curve - The model's "exam" capability on new data 🎓

### 2. ✅ Final Test Accuracy

| Experiment Configuration | Test Accuracy |
|--------------------------|---------------|
| Baseline | 0.5787 |
| Augmentation | 0.5289 |
| Dropout | 0.5604 |
| Normalization | 0.6349 |
| Aug + Dropout | 0.4767 |
| Aug + Norm | 0.5745 |
| Dropout + Norm | 0.6072 |
| Aug + Dropout + Norm | 0.5039 |
### 📈 Accuracy Curve Comparison

| | Training Phase | Validation Phase |
|--|----------------|------------------|
| **📉 Curve Type** | Training Accuracy Curve | Validation Accuracy Curve |
| **🎯 What it Shows** | Model's "practice" performance 🏋️ | Model's "exam" capability 🎓 |
| **💡 Key Insight** | How well the model learns patterns | Generalization ability on new data |

---

🚀 *Explore the code and see how these techniques transform model performance!* 

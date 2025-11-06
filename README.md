# Comparative-Analysis-of-CNN-Regularization
This project systematically compares the effects of various regularization techniques on CIFAR-10 image classification. Through eight distinct experimental configurations, it provides an in-depth analysis of how data augmentation, GroupNormalization, and Dropout—individually and in combination—impact the performance of a CNN model.

# Project Background
In deep learning image classification tasks, data augmentation can expand the diversity of training data, Dropout helps mitigate overfitting, and group normalization stabilizes the training process. This project designs multiple sets of controlled experiments to quantitatively analyze the effects of these techniques when used individually or in combination, providing references for model optimization in similar tasks.

# Tech Stack
Deep Learning Framework: TensorFlow 2.x + Keras
Dataset: CIFAR-10 (10 classes of 32×32 color images)
Visualization Tool: Matplotlib
Runtime Environment: Python 3.7+, Jupyter Notebook (or any Python IDE)

# Experimental Design
This experiment designs 8 technical combinations, covering four dimensions: "baseline model," "single technique," "dual-technique combination," and "triple-technique combination."

# Experimental Results
Accuracy Curve Comparison
Left: Training Accuracy Curve – The model's "practice" performance on the training set.
Right: Validation Accuracy Curve – The model's "exam" capability on new data (generalization ability).

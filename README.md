**📌 Project Overview**
This project develops an automated defect detection system for industrial casting products using Deep Learning and Computer Vision.

The system classifies casting products into:
✅ Defective Products
✅ Non-Defective Products

using:
- Custom Convolutional Neural Network (CNN)
- MobileNetV2 Transfer Learning
The objective is to reduce manual inspection effort and improve manufacturing quality control.

**🎯 Problem Statement**
Manual inspection of casting products is time-consuming, expensive, and prone to human error.The goal of this project is to develop an automated image classification system capable of detecting casting defects with high accuracy.

**📂 Dataset Information**
**Topic: Industrial Defect Detection**
**Casting defect detection: **Classifying the manufacturing defects accurately from images, improving product quality control.

https://www.kaggle.com/datasets/ravirajsinh45/real-life-industrial-dataset-of- casting-product

**Dataset Statistics**

| Attribute | Value |
|------------|--------|
| Dataset Name | Casting Product Image Classification Dataset |
| Domain | Industrial Manufacturing |
| Task Type | Binary Image Classification |
| Total Images | 7,348 |
| Training Images | 6,633 |
| Testing Images | 715 |
| Number of Classes | 2 |
| Image Format | JPG |
| Image Resolution | 512 × 512 pixels |
| Defective Images | 4,211 |
| Non-Defective Images | 3,137 |
| Defective Training Images | 3,758 |
| Non-Defective Training Images | 2,875 |
| Defective Testing Images | 453 |
| Non-Defective Testing Images | 262 |

**Dataset Summary**

| Metric | Value |
|---------|---------|
| Total Images | 7,348 |
| Classes | 2 |
| Training Images | 6,633 |
| Testing Images | 715 |
| Image Size | 512×512 |
| Defective Images | 4,211 |
| Non-Defective Images | 3,137 |
| Best Model | MobileNetV2 |
| Best Accuracy | 99.30% |

**🔬 Research Questions**

## RQ1

**Can a Convolutional Neural Network (CNN) accurately classify casting products as defective or non-defective?**

## RQ2

**Does MobileNetV2 transfer learning outperform a custom CNN for casting defect detection?**

## RQ3

**Which model provides better generalization performance on unseen casting images?**

## RQ4

**Can Grad-CAM explain the decision-making process of the trained MobileNetV2 model?**

#  RQ5

**Does the trained model focus on defect-related regions rather than irrelevant background features?**

**🧠 CNN Architecture**
## CNN Architecture

```text
🖼 Input Image (224×224×3)
          │
          ▼
🔵 Conv2D (32 Filters, ReLU)
          │
          ▼
🟦 MaxPooling2D
          │
          ▼
🟢 Conv2D (64 Filters, ReLU)
          │
          ▼
🟦 MaxPooling2D
          │
          ▼
🟣 Conv2D (128 Filters, ReLU)
          │
          ▼
🟦 MaxPooling2D
          │
          ▼
🟨 Flatten
          │
          ▼
🟧 Dense (128 Neurons, ReLU)
          │
          ▼
🔴 Dropout (0.5)
          │
          ▼
✅ Output Layer (1 Neuron, Sigmoid)
          │
          ▼
🎯 Prediction
(Defective / Non-Defective)
```

**🚀 Methodology**
**Data Preprocessing**
- Image Resizing (224×224)
- Pixel Normalization
- Label Encoding
**Data Augmentation**
- Rotation
- Horizontal Flip
- Zoom
- Width Shift
- Height Shift
**Models**
**Model 1**
-Custom CNN
**Model 2**
- MobileNetV2 Transfer Learning

**📊 Evaluation Metrics**
The models were evaluated using:
Accuracy
Precision
Recall
F1 Score
Confusion Matrix
Classification Report
Grad-CAM Visualization
**📈 Results**
Model                Accuracy
Custom CNN  ------->  97.90%
MobileNetV2	------->  99.30%

**Observation**
MobileNetV2 achieved the highest performance and demonstrated superior generalization capability.

**📷 Project Outputs**
Accuracy Curve

E:\CNN assign\accuracy_curve.png


Loss Curve


E:\CNN assign\loss_curve.png

Confusion Matrix

E:\CNN assign\confusion_matrix.png


Grad-CAM Visualization

E:\CNN assign\gradcam_mobilenetv2_overlay.png


**Interpretation**

The Grad-CAM visualization indicates that the model focused primarily on the defect region during classification. This suggests that the model learned meaningful defect-related features rather than relying on irrelevant background information.

**🛠 Technologies Used**
Python
TensorFlow
Keras
NumPy
Pandas
Matplotlib
Seaborn
Jupyter Notebook

**🎯 Conclusion**

This project successfully developed a deep learning-based casting defect detection system.

**Key findings:**

- Custom CNN achieved 97.9% accuracy.
- MobileNetV2 achieved 99.3% accuracy.
- Transfer learning significantly improved performance.
- Grad-CAM provided visual interpretability of model decisions.
- The system demonstrates strong potential for industrial quality inspection automation.

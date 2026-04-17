# Chest-X-ray-Disease-Classification-using-Deep-Learning
The project titled “Chest X-Ray Classification using Deep Learning and Machine Learning Techniques” focuses on developing an accurate and efficient system for detecting lung diseases, particularly pneumonia, from chest X-ray images. This project integrates both deep learning models and machine learning approaches to improve diagnostic performance and reliability.

A convolutional neural network (CNN) is used due to its strong ability to extract spatial and hierarchical features from image data.CNN is a deep learning model mainly used for image processing tasks.It automatically extracts features using convolution and pooling layers.It is widely used for classification, detection, and computer vision applications.

PCA is a dimensionality reduction technique used to simplify large datasets.It transforms features into a new set of uncorrelated variables called principal components.It helps improve model performance and reduces computational complexity.

XGBoost is an advanced ensemble learning algorithm based on gradient boosting. It builds multiple decision trees to improve prediction 
accuracy. It is widely used for structured data and high-performance models.

VGG16 is a deep convolutional neural network used for image classification tasks. It consists of 16 layers and is known for its simplicity and strong performance. It is widely used for feature extraction in transfer learning.

<img width="1489" height="784" alt="image" src="https://github.com/user-attachments/assets/e502f451-00b6-4afa-9991-39d9f5a7660b" />

This figure shows chest X-ray images from the dataset, categorized into Normal and Pneumonia classes.
It highlights visual differences used by the model to learn and classify lung conditions.

<img width="1790" height="985" alt="image" src="https://github.com/user-attachments/assets/2def07e7-9417-417d-a4ca-f74e5f09fff0" />

This figure compares accuracy, precision, recall, specificity, and F1-score of both models.The Custom CNN shows better performance than SVM across all metrics.

<img width="1489" height="990" alt="image" src="https://github.com/user-attachments/assets/d9e6d425-b8eb-4bbe-83b5-b1b95a7a09f5" />

The second part of the project, implemented in the chest X-ray classification notebook, extends the detection process by improving classification performance using advanced techniques such as transfer learning. Pre-trained models are utilized to leverage knowledge from large-scale datasets like ImageNet, enabling the system to achieve higher accuracy even with limited medical data.

PERFORMANCE ANALYSIS SUMMARY 
Best method by Accuracy:
  At 20% training data: PCA+XGBoost (0.7404)
  At 40% training data: PCA+XGBoost (0.7580)
  At 60% training data: VGG16+XGBoost (0.7628)
  At 80% training data: VGG16+XGBoost (0.7660)

Best method by F1-Score:
  At 20% training data: PCA+XGBoost (0.8262)
  At 40% training data: PCA+XGBoost (0.8353)
  At 60% training data: VGG16+XGBoost (0.8398)
  At 80% training data: VGG16+XGBoost (0.8420)

Best method by Sensitivity:
  At 20% training data: PCA+XGBoost (0.9872)
  At 40% training data: VGG16+XGBoost (0.9897)
  At 60% training data: VGG16+XGBoost (0.9949)
  At 80% training data: VGG16+XGBoost (0.9974)

Best method by Specificity:
  At 20% training data: VGG16+XGBoost (0.3333)
  At 40% training data: PCA+XGBoost (0.3846)
  At 60% training data: VGG16+XGBoost (0.3761)
  
Performance improvement from 20% to 80% training data:
  PCA+XGBoost: 0.7404 → 0.7548 (Δ 0.0144, 1.9%)
  VGG16+XGBoost: 0.7404 → 0.7660 (Δ 0.0256, 3.5%)
  Raw+XGBoost: 0.7179 → 0.7356 (Δ 0.0177, 2.5%)

In conclusion, this project successfully demonstrates the application of deep learning and machine learning techniques for chest X-ray classification. The use of CNNs enables effective feature extraction from medical images, while transfer learning improves performance with limited data.

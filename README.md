# 🧠 Image and Digit Classification – Deep Learning

This project implements deep learning models for classifying images and handwritten digits using the CIFAR-10 and MNIST datasets. The goal is to build, train, and evaluate both Artificial Neural Networks (ANN) and Convolutional Neural Networks (CNN) to understand their effectiveness on different types of visual data.

## 📂 Project Structure

Image-Classification/
├── models/ # Saved model files and checkpoints
├── notebooks/ # Jupyter notebooks for training and evaluation
├── utils/ # Helper scripts (e.g., data loaders, preprocessing)
├── data/ # Contains CIFAR-10 and MNIST datasets (downloaded)
├── outputs/ # Accuracy/loss graphs, confusion matrices, logs
├── requirements.txt # Python dependencies
├── train_ann.py # Train ANN model
├── train_cnn.py # Train CNN model
├── evaluate_model.py # Model testing and evaluation script
└── README.md # Project documentation

markdown
Copy
Edit

## 📊 Datasets Used

- **MNIST**: 70,000 grayscale handwritten digit images (28x28 pixels)
- **CIFAR-10**: 60,000 color images (32x32 pixels) across 10 categories (airplane, car, cat, etc.)

## 🧠 Models Implemented

### 1. Artificial Neural Network (ANN)
- Input layer: flattened image  
- Hidden layers: Dense layers with ReLU and Dropout  
- Output layer: Softmax over 10 classes  
- Optimizer: Adam  
- Loss: Categorical Crossentropy  

### 2. Convolutional Neural Network (CNN)
- Convolutional layers: Conv2D + ReLU + MaxPooling  
- Dense layers: Fully connected with Dropout  
- Final classifier: Softmax  
- Optimizer: Adam  
- Loss: Categorical Crossentropy  

## 📈 Training & Evaluation

- Models trained on both MNIST and CIFAR-10 datasets  
- Accuracy and loss monitored over epochs  
- Results visualized with graphs and confusion matrices  
- CNNs significantly outperformed ANNs on CIFAR-10 due to spatial feature extraction  



🔧 Technologies & Tools
Languages: Python

Libraries: TensorFlow, Keras, NumPy, Matplotlib, Scikit-learn

Concepts: Neural Networks, CNN, Dropout, ReLU, MaxPooling, Data Augmentation

🧪 Learnings & Highlights
Understood the difference in model performance across datasets of varying complexity

Learned how CNNs leverage spatial hierarchies, outperforming ANNs for image classification

Gained practical experience in model tuning, evaluation, and visualization

Built a reusable and modular deep learning training pipeline

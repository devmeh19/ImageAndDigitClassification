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

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/image-digit-classification.git
cd image-digit-classification
2. Set Up Environment
bash
Copy
Edit
pip install -r requirements.txt
3. Run Training
For ANN:
bash
Copy
Edit
python train_ann.py --dataset mnist
python train_ann.py --dataset cifar10
For CNN:
bash
Copy
Edit
python train_cnn.py --dataset mnist
python train_cnn.py --dataset cifar10
4. Evaluate Models
bash
Copy
Edit
python evaluate_model.py --model saved_model.h5 --dataset mnist
📊 Sample Results
Dataset	Model	Accuracy
MNIST	ANN	98.1%
MNIST	CNN	99.2%
CIFAR-10	ANN	~45%
CIFAR-10	CNN	78-85%

🔧 Technologies & Tools
Languages: Python

Libraries: TensorFlow, Keras, NumPy, Matplotlib, Scikit-learn

Concepts: Neural Networks, CNN, Dropout, ReLU, MaxPooling, Data Augmentation

🧪 Learnings & Highlights
Understood the difference in model performance across datasets of varying complexity

Learned how CNNs leverage spatial hierarchies, outperforming ANNs for image classification

Gained practical experience in model tuning, evaluation, and visualization

Built a reusable and modular deep learning training pipeline

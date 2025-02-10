# Convolutional Neural Network (CNN) for CIFAR-10 Classification 🖼️📊

This repository contains a Jupyter Notebook implementing a **Convolutional Neural Network (CNN)** using **TensorFlow/Keras** to classify images from the **CIFAR-10 dataset**.

## 📂 Project Structure
- `CNN.ipynb` → Main Jupyter Notebook with CNN model implementation  
- `README.md` → Project documentation  

## 📜 Dataset: CIFAR-10
The **CIFAR-10** dataset consists of **60,000 32x32 color images** in **10 classes**, with **6,000 images per class**.  
The 10 categories are:
- Airplane ✈️
- Automobile 🚗
- Bird 🐦
- Cat 🐱
- Deer 🦌
- Dog 🐶
- Frog 🐸
- Horse 🐴
- Ship 🚢
- Truck 🚛

## 🛠 Steps Performed in `CNN.ipynb`
1. **Data Loading & Preprocessing**
   - Importing **CIFAR-10 dataset** using `tensorflow.keras.datasets`
   - Normalizing pixel values to **range [0,1]** for better convergence
   - One-hot encoding the class labels  

2. **Building the CNN Model**
   - **Conv2D layers** with ReLU activation for feature extraction
   - **MaxPooling layers** to downsample feature maps
   - **Flatten layer** to convert feature maps into a vector
   - **Fully connected Dense layers** for classification
   - **Softmax activation** for multi-class output

3. **Training & Evaluation**
   - Model compilation with **categorical cross-entropy loss** and **Adam optimizer**
   - Training on CIFAR-10 dataset
   - Evaluating accuracy and loss on the test set

## 🚀 How to Run the Notebook
```bash
# Clone the repository
git clone https://github.com/ridhin006/CNN.git
cd cnn-cifar10

# Install dependencies
pip install tensorflow numpy pandas matplotlib

# Open Jupyter Notebook
jupyter notebook

# Run all cells in CNN.ipynb

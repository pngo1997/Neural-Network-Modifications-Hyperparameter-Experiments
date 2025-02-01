# 🧠 Neural Network Modifications & Hyperparameter Experiments  

## 📜 Overview  
This project involves modifying a neural network's **hyperparameters, activation functions, cost functions, and regularization methods** to improve training performance and generalization. Additionally, we conduct **experiments** to analyze the impact of different configurations on model accuracy.  

📌 **Tasks**:  
- Modify the network to support **customizable hyperparameters**.  
- Implement additional **cost functions, activation functions, and regularization methods**.  
- Add **dropout** for regularization.  
- Conduct **experiments** on the **Iris dataset** using different configurations.  

📌 **Programming Language**: `Python 3`  
📌 **Libraries Used**: `NumPy`, `pandas`, `Jupyter Notebook`  

## 🚀 1️⃣ Network Code Modifications  

### **Added Hyperparameters**  
- **Cost Functions**: Quadratic, CrossEntropy, LogLikelihood  
- **Activation Functions**: Sigmoid, Tanh, ReLU, LeakyReLU, Softmax  
- **Regularization**: L1, L2  
- **Dropout Rate**  

### **Modified Functions**  
- `set_model_parameters()` → Supports **custom cost & activation functions**.  
- `feedforward()` → Implements **dropout for hidden layers**.  
- `backprop()` → Supports **L1/L2 regularization & dropout in weight updates**.  
- `update_mini_batch()` → Incorporates **new regularization methods**.  
- `total_cost()` → Adjusted for **regularization impact on cost function**.  

📌 **Dropout Implementation**:  
- Applied **only during training** (not evaluation).  
- Uses a **binary mask** to randomly drop units.  
- Ensures **scaling to maintain expected activations**.  

## 🎯 2️⃣ Experimental Setup  

### **Dataset**  
- **Training Set**: `iris-train-2.csv`  
- **Test Set**: `iris-test-2.csv`  
- **Pretrained Models**: `iris-423.dat`, `iris4-20-7-3.dat`  

### **Experimental Parameters**  
- **Epochs**: 30  
- **Mini-batch Size**: 8  
- **Learning Rate (η)**: 0.1  
- **Regularization & Dropout**: Various configurations tested.  

📌 **Key Observations**:  
- **LeakyReLU & ReLU** show improvement over **Sigmoid/Tanh**.  
- **Regularization (L1/L2)** reduces **overfitting**.  
- **Dropout (0.3)** helps generalization but **affects training stability**.  

## 📌 Summary  
✅ Added support for multiple cost & activation functions.  

✅ Implemented L1/L2 regularization & dropout.  

✅ Modified key functions for new hyperparameters.  

✅ Conducted extensive experiments on the Iris dataset.  

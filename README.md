# Language-Learning-Assistant

>  Despite the project name, this repo demonstrates a **Convolutional Neural Network (CNN)** built using **PyTorch** to classify handwritten digits from the **MNIST dataset**.

##  Project Overview

This project is a basic implementation of a CNN model to classify digits (0–9) from the MNIST dataset. It uses two convolutional layers followed by fully connected layers. The training and testing procedures leverage the PyTorch framework.

##  Features

- Uses the MNIST dataset (downloaded automatically).
- Implements a simple CNN with dropout for regularization.
- Trains and evaluates the model on GPU if available.
- Reports accuracy and average test loss after each epoch.

##  Tech Stack

- Python
- PyTorch
- torchvision


## ⚠️ Note

- The model currently uses `F.softmax(x)` without specifying `dim`. This will raise a deprecation warning. You can fix it by using:
  
  ```python
  return F.softmax(x, dim=1)
  ```

```
.
├── data/              
├── hand-writing-recognition.ipynb           
├── README.md
```

##  Results

- Achieves ~92–93% accuracy on the MNIST test set after a few epochs.

---

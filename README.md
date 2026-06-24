# Image Processing in Intelligent Systems
## Laboratory Works Repository

**Institution:** Brest State Technical University (BSTU)  
**Department:** Intelligent Information Systems (IIT)  
**Instructor:** Assoc. Prof. A. Kroshchanka, Ph.D.

---

### 📖 Course Overview
This repository contains the laboratory assignments, source code, and report templates for the beginner course on Machine Learning and Neural Networks. The practical sessions focus on constructing, training, and evaluating neural network models using modern deep learning frameworks (primarily PyTorch) for various computer vision and data analysis tasks.

### 🗂️ Repository Structure

```text
📦 ML-Neural-Networks-Course
 ┣ 📂 Lab_01_PyTorch_Classification  # Image classification with CNNs (MNIST, CIFAR, etc.)
 ┣ 📂 Lab_02_...                     # Upcoming labs
 ┣ 📂 Templates                      # LaTeX templates for lab reports
 ┣ 📜 .gitignore
 ┣ 📜 requirements.txt
 ┗ 📜 README.md
```

---

### 🔬 Laboratory Work No. 1: Training Classifiers with PyTorch
**Objective:** Learn how to construct neural network classifiers and perform their training on well-known computer vision datasets (`torchvision.datasets`).

#### Tasks:
1. **Model Construction:** Build a Convolutional Neural Network (CNN) using basic layers (Convolutional, Linear, Pooling, ReLU).
2. **Training & Evaluation:** Train the model using the assigned dataset and optimizer (SGD, Adam, Adadelta, RMSprop). Use `CrossEntropyLoss`. Plot the training/validation loss curves using `matplotlib`.
3. **SOTA Comparison:** Compare your results with state-of-the-art architectures found in the literature.
4. **Visualization:** Implement an inference script that takes a random image from the test set and outputs the model's predicted class.

*Note: Check the `Lab_01_PyTorch_Classification` folder for your specific dataset and optimizer variant.*

---

### 🔬 Laboratory Work No. 2: Constructing Models Based on Pre-trained Neural Networks
**Objective:** Train neural networks constructed on the basis of pre-trained architectures using transfer learning techniques.

#### Tasks:
1. **Model Adaptation:** Load a designated pre-trained network (AlexNet, ResNet, MobileNet, DenseNet, SqueezeNet, ShuffleNet) and modify its final layer structure to fit the target dataset.
2. **Data Preprocessing:** Implement proper data transformation pipelines, including image resizing and converting single-channel images (MNIST, Fashion-MNIST) to 3-channel tensors to match the pre-trained model inputs.
3. **Training & Performance Evaluation:** Train the adapted network using the same optimizer from Laboratory Work 1 and `CrossEntropyLoss`. Plot the error curves.
4. **Comparative Analysis:** Compare the performance (accuracy, convergence speed) of the pre-trained model against the custom CNN architecture from Laboratory Work 1 and public SOTA benchmarks.
5. **Inference Visualization:** Implement a module to run inference on arbitrary images from the Internet using both the custom and pre-trained networks, displaying the predicted classification results.

---

### ⚙️ Installation & Setup

It is highly recommended to use a virtual environment (e.g., `venv` or `conda`) to manage dependencies.

**1. Clone the repository:**
```bash
git clone https://github.com/kroschenko/IPIS-2026.git
cd IPIS-2026
```

**2. Create a virtual environment:**
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

**3. Install the required dependencies:**
```bash
pip install -r requirements.txt
```

*Typical `requirements.txt` includes:*
```text
torch
torchvision
matplotlib
numpy
jupyter
```

---

### 📝 Submission Guidelines
For each laboratory work, students must:
1. Create a dedicated folder for the lab (e.g., `Lab_01`).
2. Include all well-commented source code (`.py` files or Jupyter Notebooks).
3. Include a compiled PDF report generated using the provided LaTeX template from the `Templates` directory.
4. Push the code to this repository before the deadline.

---
*Happy coding and training!*

AI_1
Armenian Coin Classification Using Deep Learning

Team Member:
Aleksandr Barseghyan

Project Overview

This project focuses on automatic classification of Armenian coins using Deep Learning techniques.

The system uses Convolutional Neural Networks (CNNs) to classify images of Armenian coins into their respective denominations. The model is based on the MobileNetV2 architecture, which is designed for efficient image recognition while maintaining high accuracy.

The goal of this project is to demonstrate how deep learning models can automatically recognize different coin denominations from images, which is a common computer vision task.

Repository Structure

The entire implementation is contained in a single Jupyter notebook:

AI_1/
│
├── Aleksandr_Barseghyan_armenian_coins_classification_final.ipynb
│        # Main notebook containing:
│        # - Data preprocessing
│        # - Model training
│        # - Model evaluation
│        # - Visualization of results
│
├── report.pdf
│        # Final project report
│
├── README.md
│        # Project documentation
Technologies Used
Deep Learning Frameworks

TensorFlow

PyTorch

fastai

These frameworks are used within the notebook to demonstrate different approaches to training deep learning models.

Supporting Libraries

NumPy

Matplotlib

scikit-learn

These libraries are used for data processing, visualization, and evaluation metrics.

Installation and Setup
1. Clone the Repository
git clone https://github.com/your-repository/AI_1.git
cd AI_1
2. Create a Python Environment

It is recommended to use Python 3.10 or newer.

python -m venv venv
source venv/bin/activate

For Windows:

venv\Scripts\activate
3. Install Dependencies

Install the required libraries:

pip install tensorflow
pip install torch torchvision
pip install fastai
pip install numpy matplotlib scikit-learn
pip install jupyter
Running the Project

The entire implementation is contained in the notebook:

Aleksandr_Barseghyan_armenian_coins_classification_final.ipynb

To run the project:

jupyter notebook

Then open the notebook and run the cells sequentially.

The notebook includes:

Dataset loading and preprocessing

Deep learning model training

Model evaluation

Visualization of training results

Dataset

The dataset contains images of Armenian coins from different denominations, including:

10 dram

20 dram

50 dram

100 dram

200 dram

500 dram

Images are preprocessed using:

resizing

normalization

data augmentation (rotation and flipping)

These preprocessing techniques help improve model performance and generalization.

Model Architecture

The model used in this project is based on MobileNetV2, a lightweight convolutional neural network architecture designed for efficient image classification.

Key characteristics of MobileNetV2 include:

Depthwise separable convolutions

Inverted residual blocks

Linear bottlenecks

Reduced computational complexity

This architecture provides high accuracy while remaining computationally efficient.

Training Configuration

The model is trained using the following parameters:

Parameter	Value
Optimizer	Adam
Loss Function	CrossEntropyLoss
Batch Size	32
Epochs	20–50

During training, the notebook generates:

training loss curves

validation accuracy metrics

model performance visualizations

Results Summary

The trained model achieved strong performance on the Armenian coin dataset.

Example results:

Metric	Result
Training Accuracy	~97%
Validation Accuracy	~94%
Loss	Low and stable

Evaluation methods include:

Confusion matrix

Accuracy and loss curves

Model prediction visualization

These results demonstrate that deep convolutional neural networks can effectively classify Armenian coin denominations from images.

Future Improvements

Potential improvements for this project include:

Increasing the dataset size

Applying more advanced architectures

Using object detection models for real-time coin recognition

Deploying the model as a mobile or web application

References

Relevant research and documentation used in this project include resources on:

Deep learning for computer vision

Convolutional neural networks

MobileNet architectures

Machine learning frameworks such as TensorFlow and PyTorch

Full references are included in the project report.

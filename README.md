# AI_1
Armenian Coin Classification with Deep Learning and Knowledge Representation
Team Members: Aleksandr Barseghyan

Project Overview

This project focuses on automatic classification of Armenian coins using Deep Learning techniques combined with a Knowledge Representation (KR) component.

The system uses Convolutional Neural Networks (CNNs) based on the MobileNetV2 architecture to classify images of Armenian coins into their respective denominations.

To enhance interpretability and structured reasoning, the deep learning predictions can be integrated with semantic knowledge representation using ontologies and rule-based reasoning.

The project demonstrates how perception (Deep Learning) and reasoning (Knowledge Representation) can be combined in a unified AI system.

Repository Structure
project/
│
├── data/                  # Armenian coin dataset
├── models/                # Saved trained models
├── notebooks/             # Experiments and visualization
├── src/
│   ├── train.py           # Training pipeline
│   ├── inference.py       # Prediction script
│   └── ontology_reasoning.py
│
├── report.pdf             # Final project report
├── README.md              # Project documentation
Technologies Used

Deep Learning Frameworks:

TensorFlow

PyTorch

fastai

Knowledge Representation Tools:

Protégé

Owlready2

Other Libraries:

NumPy

Matplotlib

scikit-learn

Installation and Setup
1. Clone the Repository
git clone https://github.com/your-repository/armenian-coin-classification.git
cd armenian-coin-classification
2. Create Python Environment

It is recommended to use Python 3.10+

python -m venv venv
source venv/bin/activate

Windows:

venv\Scripts\activate
3. Install Dependencies
pip install tensorflow
pip install torch torchvision
pip install fastai
pip install numpy matplotlib scikit-learn
pip install owlready2
Dataset

The dataset contains images of Armenian coins from different denominations, including:

10 dram

20 dram

50 dram

100 dram

200 dram

500 dram

Images are preprocessed through:

resizing

normalization

augmentation (rotation, flipping)

These preprocessing steps improve model generalization and robustness.

Model Architecture

The primary model used is based on:

MobileNetV2

MobileNetV2 is a lightweight CNN architecture optimized for efficient image classification, especially suitable for mobile and embedded systems.

Key characteristics:

Depthwise separable convolutions

Inverted residual blocks

Linear bottlenecks

Low computational complexity

This architecture allows the model to achieve high classification accuracy while maintaining computational efficiency.

How to Run the Project
Training the Model

To train the neural network model:

python src/train.py

Training parameters include:

Optimizer: Adam

Loss Function: CrossEntropyLoss

Batch Size: 32

Epochs: 20–50

During training, the system generates:

training loss curves

validation accuracy

saved model checkpoints

Running Inference (Prediction)

To classify new coin images:

python src/inference.py --image path_to_image.jpg

The output will display:

Predicted Class: 100 Dram
Confidence: 97.4%
Knowledge Representation Component

The project also integrates symbolic reasoning using ontologies.

An ontology describing Armenian coins can be created using:

Protégé

and processed in Python using:

Owlready2

Example reasoning rules include:

coin value hierarchy

material properties

denomination relationships

This allows the system to combine:

Neural perception + symbolic reasoning

which is part of the broader field of Neuro-Symbolic AI.

Results Summary

The model achieved strong performance on the Armenian coin dataset.

Example results:

Metric	Result
Training Accuracy	~97%
Validation Accuracy	~94%
Loss	Low and stable after convergence

Additional evaluation methods include:

Confusion Matrix

Accuracy curves

Feature map visualization

These results demonstrate that deep convolutional networks can effectively recognize Armenian coin denominations from images.

Future Improvements

Possible extensions of this work include:

Increasing dataset size

Applying object detection models such as YOLOv3

Improving interpretability using Grad-CAM

Deploying the model as a mobile application

Extending ontology reasoning for richer semantic inference

References

Key works used in this project include research on:

MobileNet architectures

Deep Learning frameworks

Neuro-symbolic AI

Semantic Web technologies

Full references are available in the project report.

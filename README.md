# Hierarchical-Intention-Recognition-Algorithm
Here is the source code related to my hierarchical intention recognition paper.

## 1. Abstract
Intention recognition is the prerequisite and foundation for achieving intelligent human‒computer interaction (IHCI). In complex task scenarios, human intentions often exhibit hierarchical and context-related characteristics. In this paper, we propose a hierarchical intention recognition framework suitable for complex tasks, aiming to infer multilevel intentions from the lowest-level data such as human behavior and contextual information. The framework's usability was validated via a case study of helicopter and drone collaborative wildfire rescue missions. First, task analysis was employed to extract the intention structure among high-level task intentions, low-level interaction intentions, and feature data. Flight simulation data from 50 complete trials conducted by 10 participants were subsequently collected. Finally, reliable recognition of interaction intentions and task intentions was achieved via the 1D-CNN+Bi-LSTM neural network and the dynamic Bayesian network (DBN) based on the "context-intention-behaviour" model. The highest recognition accuracies for interaction intentions and task intentions were 93.96% and 97.12%, respectively. The methods and results of this study provide a novel perspective for human intention recognition in complex tasks and offer methodological guidance and support for intelligent adaptive interfaces and IHCI in complex task scenarios.

## 2. Environment
Low-level interaction intention recognition model (1D-CNN+Bi-LSTM):
- Anaconda Virtual Environment with Python 3.9
- Cudnn 11.8 + PyTorch 2.1.0
- Other Python packages that may be involved: Matplotlib, Numpy, Pandas, scikit-learn, onnx, onnx-runtime
  
High-level interaction intention recognition model (Dynamic Bayesian Network):
- Anaconda Virtual Environment with Python 3.9
- SMILE academic 2.2.5, which can be accessed at [SMILE Download](https://download.bayesfusion.com/files.html?category=Academia)
- Other Python packages that may be involved: Matplotlib, Numpy, Pandas, scikit-learn, onnx, onnx-runtime



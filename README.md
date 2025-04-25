# Hierarchical-Intention-Recognition-Algorithm
Here is the source code related to my hierarchical intention recognition paper.

Paper link: https://doi.org/10.1016/j.engappai.2025.110037

## 1. Abstract
Intention recognition is the prerequisite and foundation for achieving intelligent human‒computer interaction (IHCI). In complex task scenarios, human intentions often exhibit hierarchical and context-related characteristics. In this paper, we propose a hierarchical intention recognition framework suitable for complex tasks, aiming to infer multilevel intentions from the lowest-level data such as human behaviour, machine and environmental information. The framework's usability was validated via a case study of helicopter and drone collaborative wildfire rescue missions. First, task analysis was employed to extract the intention structure among high-level task intentions, low-level interaction intentions, and feature data. Flight simulation data from 80 complete trials conducted by 16 participants were subsequently collected. Finally, reliable recognition of interaction intentions and task intentions was achieved via a one-dimensional convolutional neural network (1D-CNN) + bidirectional long short-term memory (Bi-LSTM) neural networks and a dynamic Bayesian network (DBN). The highest recognition accuracies for interaction intentions and task intentions were 94.57% and 97.33%, respectively. The methods and results of this study provide a novel perspective for human intention recognition in complex tasks and offer methodological guidance and support for intelligent adaptive interfaces and IHCI in complex task scenarios.

## 2. Environment
Low-level interaction intention recognition model (1D-CNN+Bi-LSTM):
- Anaconda Virtual Environment with Python 3.9
- Cudnn 11.8 + PyTorch 2.1.0
- Other Python packages that may be involved: Matplotlib, Numpy, Pandas, scikit-learn, onnx, onnx-runtime
  
High-level task intention recognition model (Dynamic Bayesian Network):
- Anaconda Virtual Environment with Python 3.9
- SMILE academic 2.2.5, which can be accessed at [SMILE Download](https://download.bayesfusion.com/files.html?category=Academia)
- Other Python packages that may be involved: Matplotlib, Numpy, Pandas, scikit-learn, onnx, onnx-runtime

## 3. Dataset
The dataset comprised structured data collected from 16 participants over 80 trials, as described in Section 3.3, which included 52 attributes, such as HOTAS axis information, button information, human gaze coordinates, AOI fixation, helicopter altitude, heading, drone status information, etc., resulting in nearly 1.6 million rows of sample data. The dataset covers 16 types of interaction intention labels and 5 types of task intention labels. We randomly selected 4 trials from each participant as the training set and the remaining trial as the test set. Consequently, the training set includes approximately 1,300,000 rows of samples from 64 trials, whereas the test set includes approximately 330,000 rows of samples from 16 trials.
- Original Dataset can be accessed at: https://drive.google.com/file/d/1CB3JILdEGsimUWrKVaDxW-tCbOGLEUDU/view?usp=sharing 
- Dataset for low-level interaction intention recognition can be accessed at: _Low-Level Interaction Intention Recognition\Dataset\Final_Dataset_2.csv_
- Dataset for high-level task intention recognition can be accessed at: _High-Level Task Intention Recognition\Dataset\DBN_Test_Data_2times.csv_

The tasks of the data collection process are shown in the following video:
https://drive.google.com/file/d/1t7iyEmOGsWwPB3_iopdPN-OPjZ9kg0JG/view?usp=sharing


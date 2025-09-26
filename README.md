## Foundational Concepts for Neural Networks

🚀 As part of my current studies, I have been learning the foundational concepts of neural networks. These concepts form the groundwork for the current project and provide the base before moving to the exercise and code implementation.

🔹  The learning started with the core elements of neural networks — perceptrons, multilayer perceptrons, and activation functions. This was followed by the training process, which includes forward propagation, loss computation, backpropagation, and parameter updates.

🔹  Key aspects such as loss functions and their role in guiding model learning were explored. Optimization strategies were studied, starting with gradient descent variants and extending to adaptive methods like Adam and RMSProp. Regularization techniques such as dropout, weight decay, and data augmentation were also emphasized to improve generalization.

🔹  To stabilize the training process, methods like weight initialization and batch normalization were considered. Hyperparameter tuning was highlighted as a critical practice for refining performance.

🔹  The learning further extended to well-known neural network architectures such as CNNs, RNNs, LSTMs, and Transformers, with attention to their applications in solving practical problems.

The attached visuals provide a structured overview of these components. They serve as a quick reference to the foundational knowledge that underpins the project.


|  | |
|---------|---------|
| [![Alt text 1](NN_Concepts_Quick_Reference_1.png)](NN_Concepts_Quick_Reference_1.png)|[![Alt text 2](NN_Concepts_Quick_Reference_2.png)](NN_Concepts_Quick_Reference_2.png) |

## Problem Statement

The primary objective is to develop a predictive maintenance model for wind turbine generators to reduce maintenance costs by anticipating failures before they occur. This involves building and tuning various classification models to identify generator failures before they occur. The provided dataset is a ciphered version of confidential sensor data, containing 40 predictors, with 20,000 observations in the training set and 5,000 in the test set. By accurately predicting failures (a target variable of "1"), the company can perform timely repairs (a true positive), which is more cost-effective than a full replacement (a false negative). The model must account for the cost hierarchy where inspection costs are less than repair costs, which are significantly less than replacement costs.


### Data Description

The data provided is a transformed version of the original data which was collected using sensors.

-   Train.csv - To be used for training and tuning of models.
-   Test.csv - To be used only for testing the performance of the final best model.
Both datasets consist of 40 predictor variables and 1 target variable.

### Environment Setup
**For ease of use and to avoid dependency conflicts, it is recommended to run this on Google Colab. A local setup requires manual environment configuration and dependency management.**

1. Python virtual environment:

```bash
# Create a virtual environment
python -m venv .venv

# Activate the virtual environment
# On Windows
.venv\Scripts\activate
# On macOS/Linux
source .venv/bin/activate
```

2. Install Required Packages

After activating the virtual environment, install the necessary packages listed in `requirements.txt`:
```bash
pip install -r requirements.txt
```
```bash
pip install -r requirements.txt
```

3. Deactivate the Virtual Environment

To deactivate the virtual environment, simply run:

```bash
deactivate
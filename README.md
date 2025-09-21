## Laying the Groundwork
Include Infographics

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
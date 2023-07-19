+++
title = "What is Shap?"
description = "SHAP (SHapley Additive exPlanations)"
weight = 10

+++

This guide describes what is the SHAP library used on Explainability module.

## SHAP

**SHAP (SHapley Additive exPlanations)** is a game theoretic approach to explain the output of any machine learning model. It connects optimal credit allocation with local explanations using the classic Shapley values from game theory and their related extensions (see [papers](https://github.com/slundberg/shap#citations) for details and citations) [[Github Link](https://github.com/slundberg/shap)]. 

<img src="/docs/images/explainability/shap_header.svg" alt="What is Shap?"   class="mt-3 mb-3 border border-info rounded" width="800" height="960">

The key idea behind SHAP is based on cooperative game theory, specifically the concept of Shapley values. Shapley values allocate the contribution of each player in a cooperative game by considering the value that each player adds to different coalitions. In the context of machine learning, the "players" are the features, and the "coalitions" are the subsets of features used to make predictions.

SHAP values provide a way to distribute the prediction outcome among the input features in a fair and consistent manner. This allows us to understand which features have the most significant impact on a particular prediction and how they interact with each other.

One of the main advantages of SHAP is its ability to handle complex models, including ensemble methods and deep learning models. It provides a local explanation for each prediction, allowing us to analyze the contribution of individual features in a specific instance. SHAP values can also be aggregated to provide global insights into the model's behavior and feature importance across the entire dataset.

### SHAP Installation

SHAP is already installed on our platform. For any reason, SHAP can be installed from either [PyPI](https://pypi.org/project/shap) or [conda-forge](https://anaconda.org/conda-forge/shap):

```
pip install shap
or
conda install -c conda-forge shap
```

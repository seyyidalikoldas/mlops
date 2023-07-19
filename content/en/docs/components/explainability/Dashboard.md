+++
title = "Dashboard"
description = "Explainability Dashboard"
weight = 10

+++

This guide describes how to use explainability dashboard to understand your models in our platform.

## Dashboard

The integration of explainability studies into the our platform dashboard has proven to be a valuable addition to our MLOps environments. By incorporating explainability directly into the workflow management platform, we have enhanced the interpretability and transparency of our machine learning models, enabling more informed decision-making and fostering trust in the deployed systems.

Explainability plays a crucial role in MLOps, where the seamless integration of machine learning workflows and operations is paramount.  This integration allows us to analyze and interpret our models' behavior within the same environment where we develop, train, and deploy them, streamlining our workflow and minimizing disruptions.

Through the integrated explainability features, we can gain insights into the inner workings of our models and understand the factors that drive their predictions. Visualizations and analysis tools provided by the Kubeflow dashboard empower our team to explore feature importance, identify patterns, and validate model behavior.

<img src="/docs/images/explainability/fig9_kubeflow.png" alt="Explainability Dashboard"   class="mt-3 mb-3 border border-info rounded" width="1000" height="1200">

It is a statically created dashboard for now. We will make future improvements for explainability dashboard that take the model & data and then create a dynamic dashboard with supporting to show more visualizations.

We developed model results and explainability functions for XGBoost & RandomForest models. Here's the list of supported explainability visualizations for xgboost & RandomForest Models.

| Function                                           | RandomForest Cls | RandomForest Reg | XGBoost Cls | XGBoost Reg |
| -------------------------------------------------- | :--------------: | :--------------: | :---------: | :---------: |
| Confusion Matrix                                   |     &#9745;     |                  |   &#9745;   |            |
| Squared Error Metrics                              |                  |     &#9745;     |            |   &#9745;   |
| Model's Feature Importance                         |     &#9745;     |     &#9745;     |   &#9745;   |   &#9745;   |
| Shap's Summary Plot                                |     &#9745;     |     &#9745;     |   &#9745;   |   &#9745;   |
| Global Class Explainability per each class         |     &#9745;     |                  |   &#9745;   |            |
| Global Cohort Analysis                             |                  |                  |   &#9745;   |   &#9745;   |
| Class-Based Cohort Analysis                        |     &#9745;     |                  |   &#9745;   |            |
| Showing 1k Training Sample                         |     &#9745;     |     &#9745;     |   &#9745;   |   &#9745;   |
| Class-Based Force Plot                             |     &#9745;     |                  |   &#9745;   |            |
| Partial Dependence Plot for Most Important Feature |                  |     &#9745;     |            |   &#9745;   |
| Dependence Plot for for Most Important Feature     |     &#9745;     |                  |   &#9745;   |            |
| Beeswarm Distribution                              |                  |     &#9745;     |            |   &#9745;   |
| Data-Heatmap Plot                                  |                  |     &#9745;     |   &#9745;   |   &#9745;   |

> **_NOTE:_** Many visualization methods do not support every algorithm. For example, classification and regression algorithms have different descriptions and metrics and accordingly support different visualization methods.

Some visualization of the work we plan to complete in the future.

| Function                            | Development Status |
| ----------------------------------- | :----------------: |
| Local Explainability                |   To be planned   |
| Force Plot for Local Explainability |   To be planned   |

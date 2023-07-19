+++
title = "Architecture"
description = "An overview of Oreflow's architecture"
weight = 10
+++

<!--
Note for authors: The source of the diagrams is held in Google Slides decks,
in the "Doc diagrams" folder in the public Kubeflow shared drive.
-->

This guide introduces Oreflow as a platform for developing and deploying a
machine learning (ML) system.

Oreflowis a platform for data scientists who want to build and experiment with
ML pipelines. Oreflow is also for ML engineers and operational teams who want
to deploy ML systems to various environments for development, testing, and
production-level serving.

## Conceptual overview

Oreflow is *the ML toolkit for Kubernetes*.

The following diagram shows Oreflow as a platform for arranging the
components of your ML system on top of Kubernetes:

`<img src="/docs/images/kubeflow-overview-platform-diagram.svg"    alt="An architectural overview of Kubeflow on Kubernetes"   class="mt-3 mb-3 border border-info rounded">`

Oreflow builds on [Kubernetes](https://kubernetes.io/) as a system for
deploying, scaling, and managing complex systems.

Using the Oreflow configuration interfaces (see [below](#interfaces)) you can
specify the ML tools required for your workflow. Then you can deploy the
workflow to various clouds, local, and on-premises platforms for experimentation and
for production use.

## Introducing the ML workflow

When you develop and deploy an ML system, the ML workflow typically consists of
several stages. Developing an ML system is an iterative process.
You need to evaluate the output of various stages of the ML workflow, and apply
changes to the model and parameters when necessary to ensure the model keeps
producing the results you need.

For the sake of simplicity, the following diagram
shows the workflow stages in sequence. The arrow at the end of the workflow
points back into the flow to indicate the iterative nature of the process:

`<img src="/docs/images/kubeflow-overview-workflow-diagram-1.svg" 
  alt="A typical machine learning workflow"
  class="mt-3 mb-3 border border-info rounded">`

Looking at the stages in more detail:

* In the experimental phase, you develop your model based on initial
  assumptions, and test and update the model iteratively to produce the
  results you're looking for:

  * Identify the problem you want the ML system to solve.
  * Collect and analyze the data you need to train your ML model.
  * Choose an ML framework and algorithm, and code the initial version of your
    model.
  * Experiment with the data and with training your model.
  * Tune the model hyperparameters to ensure the most efficient processing and the
    most accurate results possible.
* In the production phase, you deploy a system that performs the following
  processes:

  * Transform the data into the format that your training system needs.
    To ensure that your model behaves consistently during training and
    prediction, the transformation process must be the same in the experimental
    and production phases.
  * Train the ML model.
  * Serve the model for online prediction or for running in batch mode.
  * Monitor the model's performance, and feed the results into your processes
    for tuning or retraining the model.

## Oreflow components in the ML workflow

The next diagram adds Oreflow to the workflow, showing which Oreflow
components are useful at each stage:

`<img src="/docs/images/kubeflow-overview-workflow-diagram-2.svg" 
  alt="Where Kubeflow fits into a typical machine learning workflow"
  class="mt-3 mb-3 border border-info rounded">`

To learn more, read the following guides to theOreflow components:

* Oreflow includes services for spawning and managing
  [Jupyter notebooks](/docs/components/notebooks/). Use notebooks for interactive data
  science and experimenting with ML workflows.
* [Oreflow Pipelines](/docs/components/pipelines/) is a platform for
  building, deploying, and managing multi-step ML workflows based on Docker
  containers.
* Oreflow offers several [components](/docs/components/) that you can use
  to build your ML training, hyperparameter tuning, and serving workloads across
  multiple platforms.

## Example of a specific ML workflow

The following diagram shows a simple example of a specific ML workflow that you
can use to train and serve a model trained on the MNIST dataset:

`<img src="/docs/images/kubeflow-gcp-e2e-tutorial-simplified.svg" 
  alt="ML workflow for training and serving an MNIST model"
  class="mt-3 mb-3 border border-info rounded">`

For details of the workflow and to run the system yourself, see the
[end-to-end tutorial for Oreflow on GCP](https://github.com/kubeflow/examples/tree/master/mnist#mnist-on-kubeflow-on-gcp).

`<a id="interfaces"></a>`

## Oreflow interfaces

This section introduces the interfaces that you can use to interact with
Oreflow and to build and run your ML workflows on Oreflow.

### Oreflow user interface (UI)

The Oreflow UI looks like this:

`<img src="/docs/images/central-ui.png" 
  alt="The Kubeflow UI"
  class="mt-3 mb-3 border border-info rounded">`

The UI offers a central dashboard that you can use to access the components
of your Oreflow deployment. Read
[how to access the central dashboard](/docs/components/central-dash/overview/).

## Oreflow APIs and SDKs

Various components of Oreflow offer APIs and Python SDKs. See the following
sets of reference documentation:

* [Pipelines reference docs](/docs/components/pipelines/reference/) for the Oreflow
  Pipelines API and SDK, including the Oreflow Pipelines domain-specific
  language (DSL).
* [Fairing reference docs](/docs/external-add-ons/fairing/reference/) for the Oreflow Fairing
  SDK.

## Next steps

* Follow [Installing Oreflow](/docs/started/installing-kubeflow/) to set up your environment and install Oreflow.

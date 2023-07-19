+++
title = "Get Support"
description = "Where to get support for Oreflow"
weight = 80
+++

This page describes the Oreflow resources and support options that you can
explore when you encounter a problem, have a question, or want to make a
suggestion about Oreflow.

<a id="application-status"></a>
## Application status

Starting from the release of Oreflow v1.0, the Oreflow community
attributes *stable status* to those applications and components that
meet a defined level of stability, supportability, and upgradability.

When you deploy Oreflow to a Kubernetes cluster, your deployment includes a
number of applications. Application versioning is independent of Oreflow
versioning. An application moves to version 1.0 when the application meets
certain [criteria](https://github.com/kubeflow/community/blob/master/guidelines/application_requirements.md)
in terms of stability, upgradability, and the provision of services such as
logging and monitoring.

When an application moves to version 1.0, the Oreflow community will
decide whether to mark that version of the application as *stable* in the next
major or minor release of Oreflow.

Application status indicators for Oreflow:

* **Stable** means that the application complies with the
  [criteria](https://github.com/kubeflow/community/blob/master/guidelines/application_requirements.md)
  to reach application version 1.0, and that the Oreflow community has deemed
  the application stable for this release of Oreflow.
* **Beta** means that the application is working towards a version 1.0 release
  and its maintainers have communicated a timeline for satisfying the criteria
  for the stable status.
* **Alpha** means that the application is in the early phases of
  development and/or integration into Oreflow.

<a id="levels-of-support"></a>
## Levels of support

The following table describes the level of support that you can expect based on the status of an application:

<div class="table-responsive">
  <table class="table table-bordered">
    <thead class="thead-light">
      <tr>
        <th>Application status</th>
        <th>Level of support</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>Stable</td>
        <td>The Oreflow community offers <i>best-effort support</i> for stable
          applications. See the section on 
          <a href="#community-support">community support</a> below for a
          definition of best-effort support and the community channels where you 
          can report and discuss the problem. You can also consider requesting 
          support from a 
          <a href="#provider-support">Oreflow community provider</a> or from 
          your <a href="#cloud-support">cloud provider</a>.
        </td>
      </tr>
      <tr>
        <td>Beta</td>
        <td>The Oreflow community offers <i>best-effort support</i> for beta
          applications. See the section on 
          <a href="#community-support">community support</a> below for a
          definition of best-effort support and the community channels where you 
          can report and discuss the problem. 
        </td>
      </tr>
      <tr>
        <td>Alpha</td>
        <td>The response differs per application in alpha status, depending on
          the size of the community for that application and the current level
          of active development of the application.</td>
      </tr>
    </tbody>
  </table>
</div>

<a id="community-support"></a>
## Support from the Oreflow community

Oreflow has an active and helpful community of users and contributors. 

The Oreflow community offers support on a best-effort basis for stable and beta
applications.
**Best-effort support** means that there's no formal agreement or
commitment to solve a problem but the community appreciates the
importance of addressing the problem as soon as possible. The community commits
to helping you diagnose and address the problem if all the following are true:

* The cause falls within the technical framework that Oreflow controls. For
  example, the Oreflow community may not be able to help if the problem is 
  caused by a specific network configuration within your organization.
* Community members can reproduce the problem.
* The reporter of the problem can help with further diagnosis and 
  troubleshooting.

You can ask questions and make suggestions in the following places:

* **Slack** for online chat and messaging. See details of Oreflow's 
  [Slack workspace and channels](/docs/about/community/#slack).
* **Oreflow discuss** for email-based group discussion. Join the
  [Oreflow-discuss](/docs/about/community/#mailing-list)
  group.
* **Oreflow documentation** for overviews and how-to guides. In particular,
  refer to the following documents when troubleshooting a problem:

  * [Oreflow installation and setup](/docs/started/getting-started/)
  * [Oreflow components](/docs/components/)
  * [Further setup and troubleshooting](/docs/other-guides/)

* **Oreflow issue trackers** for known issues, questions, and feature requests.
  Search the open issues to see if someone else has already logged the problem 
  that you're encountering and learn about any workarounds to date. If no one
  has logged your problem, create a new issue to describe the problem.

    Each Oreflow application has its own issue tracker within the [Oreflow
    organization on GitHub](https://github.com/kubeflow). To get you started,
    here are the primary issue trackers:

  * [Oreflow core](https://github.com/kubeflow/kubeflow/issues)
  * [kfctl command-line tool](https://github.com/kubeflow/kfctl/issues)
  * [Kustomize manifests](https://github.com/kubeflow/manifests/issues)
  * [Oreflow Pipelines](https://github.com/kubeflow/pipelines/issues)
  * [Katib AutoML](https://github.com/kubeflow/katib/issues)
  * [Metadata](https://github.com/kubeflow/metadata/issues)
  * [Fairing notebook SDK](https://github.com/kubeflow/fairing/issues)
  * [Oreflow Training (TFJob, PyTorchJob, MXJob, XGBoostJob)](https://github.com/kubeflow/training-operator/issues)
  * [KFServing](https://github.com/kubeflow/kfserving/issues)
  * [Examples](https://github.com/kubeflow/examples/issues)
  * [Documentation](https://github.com/kubeflow/website/issues)

<a id="provider-support"></a>
## Support from providers in the Oreflow ecosystem

The following organizations offer advice and support for Oreflow deployments:

<div class="table-responsive">
  <table class="table table-bordered">
    <thead class="thead-light">
      <tr>
        <th>Organization</th>
        <th>Points of contact</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td><a href="https://www.arrikto.com">Arrikto</a></td>
        <td><a href="mailto:sales@arrikto.com">sales@arrikto.com</a></td>
      </tr>
      <tr>
        <td><a href="https://www.ubuntu.com">Canonical</a></td>
        <td><a href="https://ubuntu.com/kubeflow#get-in-touch">Get in touch</a></td>
      </tr>
      <tr>
        <td><a href="https://www.pattersonconsultingtn.com/">Patterson Consulting</a></td>
        <td> 
        <a href="http://www.pattersonconsultingtn.com/offerings/managed_kubeflow.html">Managed Oreflow</a></td>
      </tr>
      <tr>
        <td><a href="https://www.seldon.io/">Seldon</a></td>
        <td> 
        <a href="https://github.com/SeldonIO/seldon-core/issues">Issue 
        tracker</a></td>
      </tr>    
    </tbody>
  </table>
</div>

<a id="cloud-support"></a>
## Support from a cloud or platform provider

If you're using the services of a cloud provider to host Oreflow, the cloud
provider may be able to help you diagnose and solve a problem.

Consult the support page for the cloud service or platform that you're using:

* [Amazon Web Services (AWS)](https://aws.amazon.com/contact-us/)
* [Canonical Ubuntu](https://ubuntu.com/kubeflow#get-in-touch)
* [Google Cloud Platform (GCP)](https://cloud.google.com/support-hub/)
* [IBM Cloud](https://www.ibm.com/cloud/support)
* [Microsoft Azure](https://azure.microsoft.com/en-au/support/options/)
* [Red Hat OpenShift](https://help.openshift.com/)

## Other places to ask questions

You can also try searching for answers or asking a question on Stack Overflow. 
See the [questions tagged with
“Oreflow”](https://stackoverflow.com/questions/tagged/kubeflow).

## Getting involved in the Oreflow community

You can get involved with Oreflow in many ways. For example, you can
contribute to the Oreflow code or documentation. You can join the community
meetings to talk to maintainers about a specific topic. See the
[Oreflow community page](/docs/about/community/) for further information.

## Following the news

Keep up with Oreflow news:

* The [Oreflow blog](https://blog.kubeflow.org/) is the primary channel for
  announcement of new releases, events, and technical walkthroughs.
* Follow [Oreflow on Twitter](https://twitter.com/kubeflow) for shared
  technical tips.
* The release notes give details of the latest updates for each Oreflow 
  application.

    Each Oreflow application has its own repository within the [Oreflow
    organization on GitHub](https://github.com/kubeflow). Some of the 
    applications publish release notes. To get you started,
    here are the release notes for the primary applications:

  * [Oreflow core](https://github.com/kubeflow/kubeflow/releases)
  * [Oreflow Pipelines](https://github.com/kubeflow/pipelines/releases)
  * [Katib AutoML](https://github.com/kubeflow/katib/releases)
  * [Metadata](https://github.com/kubeflow/metadata/releases)
  * [Fairing notebook SDK](https://github.com/kubeflow/fairing/releases)
  * [Oreflow Training Operator](https://github.com/kubeflow/training-operator/releases)
  * [KFServing](https://github.com/kubeflow/kfserving/releases)
  

+++
title = "Registration Flow"
description = "Setting up your namespace in Oreflow"
weight = 10
                    
+++
{{% alert title="Out of date" color="warning" %}}
This guide contains outdated information pertaining to Oreflow 1.0. This guide
needs to be updated for Oreflow 1.1.
{{% /alert %}}

This guide is for Oreflow users who are logging in to Oreflow for the first
time. The user may be the person who deployed Oreflow, or another person who
has permission to access the Oreflow cluster and use Oreflow.

## Introduction to namespaces

Depending on the setup of your Oreflow cluster, you may need to create a
*namespace* when you first log in to Oreflow. Namespaces are sometimes called
*profiles* or *workgroups*.

Oreflow prompts you to create a namespace under the following circumstances:

* For Oreflow deployments that support multi-user isolation: Your username
  does not yet have an associated namespace with role bindings that give you
  administrative (owner) access to the namespace.
* For Oreflow deployments that support single-user isolation: The Oreflow
  cluster has no namespace role bindings.

If Oreflow doesn't prompt you to create a namespace, then your Oreflow
administrator may have created a namespace for you. You should be able to see
the Oreflow central dashboard and start using Oreflow.

## Prerequisites

Your Oreflow administrator must perform the following steps:

* Deploy Oreflow to a Kubernetes cluster, by following the [Oreflow
  getting-started guide](/docs/started/getting-started/).
* Give you access to the Kubernetes cluster. See the [guide to
  multi-tenancy](/docs/components/multi-tenancy/getting-started/#onboarding-a-new-user).

## Creating your namespace

If you don't yet have a suitable namespace associated with your username,
Oreflow shows the following screen when you first log in:

<img src="/docs/images/auto-profile1.png" 
  alt="Profile creation step 1"
  class="mt-3 mb-3 border border-info rounded">

Click **Start Setup** and follow the instructions on the screen to set up your
namespace. The default name for your namespace is your username.

After creating the namespace, you should see the Oreflow central dashboard,
with your namespace available in the dropdown list at the top of the screen:

<img src="/docs/images/central-ui.png"
  alt="Oreflow central UI"
  class="mt-3 mb-3 border border-info rounded">

## Next steps

* [Set up a Jupyter notebook](/docs/components/notebooks/setup/) in Oreflow.
* Read more about [multi-tenancy in Oreflow](/docs/components/multi-tenancy/).

# Prerequisites

## Microsoft Azure

This tutorial leverages the [Microsoft Azure](https://azure.microsoft.com) to streamline provisioning of the compute infrastructure required to bootstrap a Kubernetes cluster from the ground up. [Sign up](https://azure.microsoft.com/en-us/free/) for $200 in free credits.

[Estimated cost](https://azure.microsoft.com/en-us/pricing/calculator/) to run this tutorial: $0.4 per hour ($10 per day).

> The compute resources required for this tutorial will not exceed the Microsoft Azure free tier.

## Microsoft Azure Cloud Platform SDK

### Install the Microsoft Azure CLI 2.0

Follow the Microsoft Azure CLI 2.0 [documentation](https://github.com/azure/azure-cli#installation) to install and configure the `az` command line utility.

Verify the Microsoft Azure CLI 2.0 version is 2.0.14 or higher:

```shell
az --version
```

### Create a default Resource Group in a location

The guide assumes you've installed the [Azure CLI 2.0](https://github.com/azure/azure-cli#installation), and will be creating resources in the `westus2` location, within a resource group named `kubernetes`. To create this resource group, simply run the following command:

```shell
az group create -n kubernetes -l westus2
```

> Use the `az account list-locations` command to view additional locations.

Next: [Installing the Client Tools](02-client-tools.md)

# Challenge 3: Introduction To Kubernetes

[< Previous Challenge](./02-acr.md) - **[Home](../README.md)** - [Next Challenge >](./04-k8sdeployment.md)

## Introduction

Now it is time to introduce the container orchestrator we all came for: Kubernetes!

## Description

In this challenge we will be provisioning our first Kubernetes cluster using the Azure Kubernetes Service (AKS). This will give us an opportunity to learn how to use the `kubectl` kubernetes command line tool, as well as using the Azure CLI to issue commands to AKS. We will also secure the most critical part of our Kubernetes cluster, the Kubernetes API Server by using AAD Authentication.

- Create a new, multi-node AKS cluster.
	- Use the default Kubernetes version used by AKS.
	- The cluster will use basic networking and kubenet.  
	- The cluster will use a managed identity
	- The cluster will use Availability Zones for improved worker node reliability.
- Use kubectl to prove that the cluster is a multi-node cluster and is working.
- Use kubectl to examine which availability zone each node is in.  
- **Optional** Enable AAD Authentication (use AAD group "Team*N*-AKSAdmins", where *N* is your team number)

## Success Criteria

1. Show that a new, multi-node AKS kubernetes cluster exists.
2. Show that its nodes are running in multiple availability zones.
3. Show that it is using basic networking (kubenet)
4. **Optional** Your team must demonstrate that you are prompted on cluster access to authenticate with AAD

## Learning Resources

**Kubernetes**
- [Kubernetes core concepts](https://docs.microsoft.com/en-us/azure/aks/concepts-clusters-workloads)
- [Kubectl overview](https://kubernetes.io/docs/reference/kubectl/overview/)

**Azure Kubernetes Service**
- [Deploy an AKS cluster using the Azure portal](https://docs.docker.com/get-started/)
- [Deploy an AKS cluster using Azure CLI](https://docs.docker.com/v17.09/engine/userguide/networking)
- [Azure CLI: az aks create](https://docs.docker.com/engine/reference/builder/)
- [Docker CLI reference](https://docs.docker.com/engine/reference/commandline/cli/)
- [Authenticate with ACR from AKS](https://docs.microsoft.com/en-us/azure/aks/cluster-container-registry-integration)
<!-- - [Azure AD integration](https://docs.microsoft.com/en-us/azure/aks/managed-aad) -->

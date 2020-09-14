# Intro To Kubernetes
## Introduction
This intro level hack will help you get hands-on experience with Docker, Kubernetes and the Azure Kubernetes Service (AKS) on Microsoft Azure. Kubernetes has quickly gone from being the shiny new kid on the block to the defacto way to deploy and orchestrate containerized applications.

This hack starts off by covering containers, what problems they solve, and why Kubernetes is needed to help orchestrate them.  You will learn all of the Kubernetes jargon (pods, services, and deployments, oh my!).  By the end, you should have a good understanding of what Kubernetes is and be familiar with how to run it on Azure.


## Learning Objectives
In this hack you will solve a common challenge for companies migrating to the cloud. You will take a simple multi-tiered web app, containerize it, and deploy it to an AKS cluster. Once the application is in AKS, you will learn how to tweak all the knobs and levers to scale, manage and monitor it.

1. Containerize an application
1. Deploy a Kubernetes cluster in Azure and deploy applications to it.
1. Understand key Kubernetes management areas: scalability, upgrades and rollbacks, storage, networking, package management and monitoring

## Challenges
- Challenge 1: **[Got Containers?](Challenges/01-containers.md)**
   - Package the "FabMedical" app into a Docker container and run it locally.
- Challenge 2: **[The Azure Container Registry](Challenges/02-acr.md)**
   - Deploy an Azure Container Registry, secure it and publish your container.
- Challenge 3: **[Introduction To Kubernetes](Challenges/03-k8sintro.md)**
   - Install the Kubernetes CLI tool, deploy an AKS cluster in Azure, and verify it is running.
- Challenge 4: **[Your First Deployment](Challenges/04-k8sdeployment.md)**
   - Pods, Services, Deployments: Getting your YAML on! Deploy the "FabMedical" app to your AKS cluster. 
- Challenge 5: **[Scaling and High Availability](Challenges/05-scaling.md)**
   - Flex Kubernetes' muscles by scaling pods, and then nodes. Observe how Kubernetes responds to resource limits.
- Challenge 6: **[Deploy MongoDB to AKS](Challenges/06-deploymongo.md)**
   - Deploy MongoDB to AKS from a public container registry.
- Challenge 7: **[Updates and Rollbacks](Challenges/07-updaterollback.md)**
   - Deploy v2 of FabMedical to AKS via rolling updates, roll it back, then deploy it again using the blue/green deployment methodology.
- Challenge 8: **[Helm](Challenges/08-helm.md)**
   - Install Helm tools, customize a sample Helm package to deploy FabMedical, publish the Helm package to Azure Container Registry and use the Helm package to redeploy FabMedical to AKS.
- Challenge 9: **[Networking](Challenges/09-networking.md)**
   - Explore different ways of routing traffic to FabMedical by configuring an Ingress Controller.
- Challenge 10: **[Operations and Monitoring](Challenges/10-opsmonitoring.md)**
   - Explore the logs provided by Kubernetes using the Kubernetes CLI, configure Azure Monitor and build a dashboard that monitors your AKS cluster
  

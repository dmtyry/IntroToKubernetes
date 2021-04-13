# Challenge 5: Scaling and High Availability

[< Previous Challenge](./04-k8sdeployment.md) - **[Home](../README.md)** - [Next Challenge >](./06-deploymongo.md)

## Introduction

Now that you have your application running there are a few things to consider. How do you make it responsive? How do you make it resilient? How do you control costs while mananging load? In this challenge, we'll find that out.

## Description

In this challenge we will cover scale and resiliency from multiple aspects. We'll make sure enough replicas of our container are running to handle load. We'll make sure that there are enough resources in our cluster to handle all the containers we want to run and we'll figure out how Kubernetes repairs itself.

- Scale the nodes in the AKS cluster from 3 to 1.  Make sure you watch the pods after you perform the scale operation.  
- Scale the **Web** app to 2 instances
- Scale the **API** app to 4 instances using the same technique as above.  
- Watch events using kubectl with its special watch option (the docs are your friend!).
	- You will find an error occurs because the cluster does not have enough resources to support that many instances.
	- There are three ways to fix this: increase the size of your cluster, decrease the resources needed by the deployments or deploy the cluster autoscaler to your cluster. 
- To fully deploy the application, you will need 4 instances of the API app running and 2 instances of the Web app. 
	- Hint: If you fixed the issue above correctly (look at pod resource request!), you should be able to do this with the resources of your original cluster.
- When your cluster is fully deployed, browse to the “/stats.html” page of the web application.
	- Keep refreshing to see the API app’s host name keep changing between the deployed instances.
- Scale the API app back down to 1, and immediately keep refreshing the `/stats.html` page.
	- You will notice that without any downtime it now directs traffic only to the single instance left.

## Success Criteria

1. You can successfully scale your cluster down to 1 node.
1. At least 2 replicas of content-web is running.
1. At least 4 replicas of content-api is running.
1. Fix the resource issues if so.
1. Cluster autoscaler enabled and tested

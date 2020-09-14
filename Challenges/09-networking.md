# Challenge 09: Networking

[< Previous Challenge](./08-helm.md) - **[Home](../README.md)** - [Next Challenge >](./10-opsmonitoring.md)

## Introduction

We started out with some very simple, default networking that Kubernetes gives us for free. But this is rarely what we'll need to go into production. Now we'll get a little more in depth on networking in Kubernetes

## Description

In this challenge you will be installing an Ingress Controller and learning how the "Ingress" resource in Kubernetes works. 

- Delete the existing content-web deployment and service.
- Install the nginx ingress controller.
- Deploy the content-web service and create an Ingress resource for it. 
- **Optional** Enable SSL/TLS on the front-end ingress

## Success Criteria

1. The nginx Ingress Controller is installed in your cluster
1. You've recreated a new Ingress for content-web that allows access through a domain name.


## References

[Ingress](https://kubernetes.io/docs/concepts/services-networking/ingress/)

[Ingress Controllers](https://kubernetes.io/docs/concepts/services-networking/ingress-controllers/)

[Create an NGINX ingress controller in AKS](https://docs.microsoft.com/en-us/azure/aks/ingress-basic)

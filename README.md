# Using vRA to deploy vSphere with Tanzu Namespaces & Guest Clusters
This repository contains the code used to create the contructs for deploying vSphere with Tanzu Supervisor Namespaces and Guest Clusters. 

## High Level Steps

To achieve our requirements, we’ll be configuring the following:

    Cloud Assembly
        VCF SDDC Manager Integration
        Kubernetes Cloud Zone – Tanzu Supervisor Cluster
        Cloud Template to deploy a new Tanzu Supervisor Namespace
    Code Stream
        Tasks to provision a new Supervisor Namespace using the Cloud Assembly Template
        Tasks to provision a new Tanzu Guest Cluster inside of the Supervisor namespace using CI Tasks and the kubectl command line tool
        Tasks to create a service account inside of the Tanzu Guest Cluster
        Tasks to create Kubernetes endpoint for the new Tanzu Guest Cluster in both Cloud Assembly and Code Stream
    Service Broker
        Catalog Item to allow End-Users to provision a brand new Tanzu Guest Cluster in its own Supervisor Namespace


To get started, please see this blog post:
- https://veducate.co.uk/vra-deploy-tanzu-clusters/ 

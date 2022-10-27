# Smokeping On Kubernetes
Working implementation of Smoke ping in kuberentes. Uses persistent volumes, kustomize and a wierd init container for merging in custom targets. 

I wrote this for my personal PI cluster, you may notice that there are references to pi everywhere. 

## Setup

This setup assumes that:

You have Kuberentes ( k8s/k3s ).
You have a dedicated storage for a persistent volume claim. ( a usb drive in OP's case.  )


### Storage configuration:

You really don't need much it's based in how long you want to store the data. 

There's two storage points:
- Data
- Config

Respectively located under storage/. You will need to update the mount points

## References 
[Smokeping Project] (https://oss.oetiker.ch/smokeping/)
[Linuxserver.io Dockerised Images] (https://hub.docker.com/r/linuxserver/smokeping)

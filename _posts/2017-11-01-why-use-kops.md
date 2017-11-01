---
layout: post
title: "> Why use Kops"
excerpt_separator: "<!--more-->"
categories:
  - kubernetes
tags:
  - kops
  - aws
---
`kops` is a tool that creates a Kubernetes clusters and help you maintain/update it.

Here is the project page for kops: https://github.com/kubernetes/kops

Creating and maintaining a Kubernetes cluster has always been hard and it is just
getting harder because there are more and more features added which requires more
configurations.  While you should understand how your cluster works,
I think it is not reasonable to have each operator understand everything about it.
That will make it unscalable.

`kops` provides a configuration driven way for you to provision a cluster and
be able to update it throughout the cluster's lifetime in a safe and predictable manor.

## Documentation
One of the most important thing about a project is documentation.  If you cant
find information about what it can do and how to do it without looking at the code,
that makes it very hard to use.  

`kops` is very well documented.  Almost every feature has various examples on usage
with cli commands included.

## Creation
You


## Network
Cluster creation and provisioning is highly configurable.  You can tell `kops` to
place this cluster in a specific VPC, specify AWS availability zones, IP ranges for
each subnets, and many more options.

## Cluster config yaml


## Updating




\-------------------------------------------------------------------------------

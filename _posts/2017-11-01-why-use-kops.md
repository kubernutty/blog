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

## Should you use it?

I think if you dont need a super customized Kubernetes cluster then you should use `kops`.  When I say "super customized" it would be stuff like running an OS that `kops` does not support or if you need to install something onto the base OS.

I also think that as a first swag at your application, use `kops` to bring up a Kubernetes cluster.  Put your app on there and try it out.  A lot of the time you dont need to customize too much because your application is Dockerized already and it is agnostic to what runs it.

If after running your application on a cluster that `kops` built for you doesnt work for some reason and you have determined that you need to build your own cluster, not much time is lost.  Mostly all of your Kubernetes application configuration files will work on your new cluster with zero to almost zero changes.

I would argue even if you think it will not work, I would prototype it on a cluster brought up by `kops` first.  The big reason is that you dont have to maintain creating and upgrading the cluster.  The good folks at `kops` is doing all that for you and testing it out.


\-------------------------------------------------------------------------------

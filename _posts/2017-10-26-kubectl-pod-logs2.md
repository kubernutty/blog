---
layout: post
title: "kubectl Pod logs"
excerpt_separator: "<!--more-->"
categories:
  - kubernetes
tags:
  - kubectl
  - logs
  - pods
---
Foo bar

### tailing

This will tail and follow the pod's logs

```
kubectl -f <pod_name>
```

### Showing the last X number of lines

When a pod has been running for a while, the logs can be very long.  You probably
only want to see the last few lines.

```
kubectl --tail=10 <pod_name>
```

### Combining options

You can combine the follow and last x number of lines options

```
kubectl -f --tail=10 <pod_name>
```

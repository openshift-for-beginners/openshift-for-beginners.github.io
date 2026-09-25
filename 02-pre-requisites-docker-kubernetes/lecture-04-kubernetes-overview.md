---
layout: page
title: "Lecture 4: Kubernetes Overview"
permalink: /02-pre-requisites-docker-kubernetes/lecture-04-kubernetes-overview/
---

# Lecture 4: Kubernetes Overview

## Overview

Once applications are packaged as containers, the next challenge is managing them at scale.  
This is where Kubernetes becomes important.

Kubernetes is a container orchestration platform that helps deploy, manage, scale, and monitor containerized applications across clusters of machines.

It is the foundation on which OpenShift is built.

---

## Learning Objectives

After this topic, I should be able to:

- explain what Kubernetes is
- understand why container orchestration is needed
- identify key Kubernetes concepts
- describe how Kubernetes supports scaling and reliability
- connect Kubernetes concepts to OpenShift

---

## Why Kubernetes is Needed

Running a single container is simple.

But real-world applications often require:

- multiple containers
- multiple servers
- service discovery
- load balancing
- scaling
- self-healing
- rolling updates
- configuration management

Managing all of this manually becomes difficult very quickly.

Kubernetes solves this by automating container orchestration.

---

## What is Kubernetes?

Kubernetes is an open-source platform used to:

- deploy containerized applications
- manage application lifecycle
- scale workloads
- recover failed containers
- distribute workloads across nodes
- expose services
- support declarative infrastructure

A simpler way to think about it:

> Kubernetes makes sure the desired application state matches the actual running state.

---

## Core Kubernetes Idea

In Kubernetes, I declare what I want:

- how many application instances should run
- which container image to use
- how the app should be exposed
- what resources it needs

Kubernetes continuously works to maintain that desired state.

---

## Important Kubernetes Concepts

### 1. Cluster
A Kubernetes cluster is a group of machines that run containerized applications.

It usually includes:

- control plane components
- worker nodes

### 2. Node
A node is a machine in the cluster that runs workloads.

### 3. Pod
A Pod is the smallest deployable unit in Kubernetes.

A Pod usually contains:

- one or more containers
- shared network
- shared storage context

In most cases, one application container runs per pod.

### 4. Deployment
A Deployment manages pods and ensures the desired number of replicas are running.

It supports:

- rolling updates
- rollback
- scaling

### 5. Service
A Service provides a stable way to access pods, even when pod IPs change.

### 6. Namespace
A Namespace logically separates resources inside a cluster.

In OpenShift, this concept is closely related to **Projects**.

---

## Example Problem Kubernetes Solves

Suppose an application should always have **3 running instances**.

If one container crashes:

- without orchestration, someone must restart it manually
- with Kubernetes, the system automatically creates a replacement

This is called **self-healing**.

---

## Common Kubernetes Capabilities

### Self-Healing
If a pod fails, Kubernetes recreates it.

### Scaling
Applications can scale up or down based on need.

### Load Balancing
Traffic can be distributed across application instances.

### Rolling Updates
New application versions can be rolled out gradually.

### Declarative Management
You define desired state in YAML, and Kubernetes enforces it.

---

## YAML in Kubernetes

Kubernetes commonly uses YAML manifests to define resources such as:

- pods
- deployments
- services
- config maps
- secrets

Example structure:

```yaml
apiVersion: apps/v1
kind: Deployment
metadata:
  name: myapp
spec:
  replicas: 2
```

This declarative style is also heavily used in OpenShift.

---

## Basic Kubernetes Workflow

A simple application deployment flow in Kubernetes looks like this:

1. Create a deployment
2. Kubernetes creates pods
3. Create a service
4. Traffic reaches the pods through the service
5. Scale the deployment when needed

---

## Kubernetes and OpenShift

This is one of the most important relationships to understand.

### Kubernetes provides:
- pods
- deployments
- services
- replica management
- scheduling
- scaling
- namespaces

### OpenShift adds:
- routes
- projects
- image streams
- build configs
- stronger opinionated security defaults
- web console
- developer-friendly workflows

So OpenShift is not separate from Kubernetes.  
It is built on Kubernetes and extends it.

---

## Common `kubectl` Style Thinking vs OpenShift `oc`

In Kubernetes, people often use:

```bash
kubectl get pods
kubectl get deployments
kubectl get services
```

In OpenShift, the equivalent CLI is usually:

```bash
oc get pods
oc get deployments
oc get services
```

This similarity shows how closely OpenShift aligns with Kubernetes concepts.

---

## Key Takeaways

- Kubernetes is a container orchestration platform
- It manages deployment, scaling, recovery, and service exposure
- Pods are the smallest deployable units
- Deployments manage pods
- Services expose workloads inside the cluster
- OpenShift is built on Kubernetes and extends it

---

## My Notes

### What seems important
- desired state model
- pods as the smallest unit
- deployments for managing replicas
- services for stable access
- namespaces as logical isolation

### Topics to explore deeper later
- difference between deployment and deployment config
- how OpenShift projects relate to namespaces
- how routes extend service exposure
- autoscaling in OpenShift

---

## Quick Summary

Kubernetes is the orchestration engine that manages containerized applications at scale.  
It automates deployment, scaling, service discovery, and self-healing.  
Since OpenShift is built on Kubernetes, understanding these basics is essential.

---

## Navigation

- [← Previous Topic: Docker Overview]({{ site.baseurl }}/02-pre-requisites-docker-kubernetes/lecture-03-docker-overview/)
- [Back to Section 2]({{ site.baseurl }}/02-pre-requisites-docker-kubernetes/)
- [Next Section: Getting Started with OpenShift →]({{ site.baseurl }}/03-getting-started-openshift/)

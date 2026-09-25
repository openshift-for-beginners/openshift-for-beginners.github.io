---
layout: page
title: "Lecture 2: OpenShift Introduction"
permalink: /01-introduction/lecture-02-openshift-introduction/
---

# Lecture 2: OpenShift Introduction

## Overview

This lecture introduces OpenShift at a high level. It explains what OpenShift is, why it is used, and how it builds on top of Kubernetes to provide a more complete enterprise platform.

## Learning Objectives

After this lecture, I should be able to:

- Define OpenShift
- Explain how OpenShift relates to Kubernetes
- Identify important OpenShift capabilities
- Understand why teams use OpenShift in enterprise environments

## What is OpenShift?

OpenShift is a Kubernetes-based container application platform. It helps teams build, deploy, manage, and scale applications using containers.

In simple terms:

- **Docker** helps package applications into containers
- **Kubernetes** helps orchestrate containers
- **OpenShift** adds enterprise-ready tools, workflows, security, and developer experience on top of Kubernetes

## Simple Definition

OpenShift can be understood as:

> A platform built on Kubernetes that simplifies application deployment and cluster operations for developers and administrators.

## Why OpenShift is Useful

OpenShift is useful because it provides more than raw container orchestration. It includes features that help with:

- application deployment
- CI/CD workflows
- image management
- routing and exposure of services
- access control
- security policies
- developer and administrator tooling

## OpenShift vs Kubernetes

OpenShift uses Kubernetes at its core, but adds several platform features and opinionated defaults.

### Kubernetes provides:
- pod orchestration
- deployments
- services
- scaling
- cluster scheduling

### OpenShift adds:
- web console
- integrated image streams
- build configurations
- routes
- stronger default security controls
- developer-focused workflows
- enterprise management features

## Core OpenShift Ideas

### 1. Container Platform
Applications are packaged as containers and run consistently across environments.

### 2. Kubernetes Foundation
OpenShift uses Kubernetes objects and concepts such as:
- pods
- services
- deployments
- namespaces
- config maps
- secrets

### 3. Developer Experience
OpenShift makes it easier for developers to:
- deploy apps from source or images
- use the web console
- build images automatically
- expose applications externally

### 4. Operations and Governance
OpenShift supports administrators with:
- user and project management
- RBAC
- quotas and limits
- security policies
- cluster-wide controls

## Common OpenShift Components Mentioned in Beginner Courses

Some OpenShift-specific components you will likely encounter later in the course include:

- **Projects** – OpenShift’s working unit, similar to Kubernetes namespaces
- **Routes** – used to expose services externally
- **Image Streams** – track and manage container images
- **BuildConfig** – define how application images are built
- **DeploymentConfig** – OpenShift-style deployment object used in many classic workflows

## Typical OpenShift Use Cases

OpenShift is commonly used for:

- hosting internal enterprise applications
- managing microservices
- standardizing deployment workflows
- enabling developer self-service
- implementing secure multi-team environments
- supporting CI/CD pipelines

## High-Level Workflow in OpenShift

A basic application lifecycle in OpenShift often looks like this:

1. Developer pushes source code
2. OpenShift builds a container image
3. The image is stored and tracked
4. The application is deployed to the cluster
5. A service exposes it internally
6. A route exposes it externally
7. The app can then be scaled and managed

## Benefits of Learning OpenShift

Learning OpenShift helps me understand:

- modern application platforms
- container orchestration in enterprise environments
- Kubernetes plus platform services
- DevOps-oriented deployment workflows
- secure and scalable application management

## Key Terms Introduced

### OpenShift
A Kubernetes-based application platform.

### Container
A lightweight package containing an application and its dependencies.

### Kubernetes
A container orchestration system.

### Route
An OpenShift resource used to expose an application outside the cluster.

### Project
An OpenShift organizational boundary for resources, similar to a namespace.

## Key Takeaways

- OpenShift is built on Kubernetes
- It provides additional tools for developers and administrators
- It simplifies deployment, security, and application exposure
- It is commonly used in enterprise environments
- Understanding Docker and Kubernetes basics will make OpenShift easier to learn

## My Notes

### What seems important
- OpenShift is not a replacement for Kubernetes; it extends it
- OpenShift has its own platform-level abstractions
- Many future topics in the course will build on this introduction

### Topics I want to explore deeper later
- Image Streams
- BuildConfig
- DeploymentConfig
- Routes
- RBAC
- SCC

## Quick Summary

OpenShift is an enterprise container platform built on Kubernetes. It helps teams build, deploy, secure, and manage applications more efficiently by adding platform services and developer-friendly workflows on top of Kubernetes.

## Next Step

Continue to the next section on Docker and Kubernetes prerequisites.

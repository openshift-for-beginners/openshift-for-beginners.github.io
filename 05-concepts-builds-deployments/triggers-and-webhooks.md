---
layout: page
title: "Triggers and Webhooks"
permalink: /05-concepts-builds-deployments/triggers-and-webhooks/
---

# Triggers and Webhooks

Automation is a key feature of OpenShift builds and deployments.

## 1. Triggers
Triggers allow a build or deployment to start automatically based on an event:
- **Image Change Trigger:** Start a build/deploy when a base image or application image is updated.
- **Config Change Trigger:** Start a build/deploy when the definition (YAML) of the resource changes.

## 2. Webhooks
Webhooks allow external systems to tell OpenShift to start a build:
- **GitHub/GitLab Webhooks:** When you `git push` code, GitHub sends a signal to OpenShift to start a new build.
- **Generic Webhooks:** Trigger builds from any third-party CI tool.

---

## Navigation
- [← Previous: Build Strategies]({{ site.baseurl }}/05-concepts-builds-deployments/build-strategies/)
- [Next: Routes Overview →]({{ site.baseurl }}/05-concepts-builds-deployments/routes-overview/)
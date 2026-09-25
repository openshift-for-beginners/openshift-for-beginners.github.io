---
layout: page
title: "Lecture 23: Demo - Build and Build Config"
permalink: /05-concepts-builds-deployments/lecture-23-demo-build-and-buildconfig/
---

# Lecture 23: Demo - Build and Build Config

This demo covers how to interact with builds using the OpenShift CLI.

### 1. View BuildConfigs
To see the build definitions in your project:
```bash
oc get bc
```

### 2. Start a New Build
If you have updated your code and want to trigger a manual build:
```bash
oc start-build <buildconfig-name>
```

### 3. Track Build Progress
To see the history of all builds:
```bash
oc get builds
```

### 4. View Build Logs
If a build is failing, the logs are the first place to look:
```bash
oc logs -f build/<build-name>
```

---

## Navigation
- [← Previous: Lecture 22]({{ site.baseurl }}/05-concepts-builds-deployments/lecture-22-build-and-buildconfig-overview/)
- [Next Topic: Lecture 24 - Route Overview →]({{ site.baseurl }}/05-concepts-builds-deployments/lecture-24-route-overview/)
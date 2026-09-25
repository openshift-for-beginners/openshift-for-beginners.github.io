---
layout: page
title: "Lecture 19: Demo - Deployment Config/Deployment"
permalink: /05-concepts-builds-deployments/lecture-19-demo-deploymentconfig-deployment/
---

# Lecture 19: Demo - Deployment Config/Deployment

This demo shows how to view and identify the different deployment types in the CLI.

### Step 1: List Deployments
To see standard Kubernetes deployments:
```bash
oc get deployments
```

### Step 2: List DeploymentConfigs
To see OpenShift-specific deployment configs:
```bash
oc get dc
```

### Step 3: Inspect the Differences
If you describe a `DeploymentConfig`, you can see the "Triggers" section which is unique to OpenShift:
```bash
oc describe dc <name>
```

Look for the `Triggers` and `Strategy` sections in the output. These define how OpenShift handles automated rollouts.

---

## Navigation
- [← Previous: Lecture 18]({{ site.baseurl }}/05-concepts-builds-deployments/lecture-18-deploymentconfig-vs-deployment/)
- [Next Topic: Lecture 20 - Image Streams Overview →]({{ site.baseurl }}/05-concepts-builds-deployments/lecture-20-image-streams-overview/)
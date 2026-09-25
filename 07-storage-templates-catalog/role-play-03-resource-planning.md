---
layout: page
title: "Role Play 3: Resource Planning for Teams"
permalink: /07-storage-templates-catalog/role-play-03-resource-planning/
---

# Role Play 3: Resource Planning for Teams

### Scenario
You are the cluster administrator. A new team is joining the cluster and they need a project to host their 5 microservices.

### Discussion
- **Storage:** Does the team need data to persist? If so, we need to ensure a **StorageClass** is available for dynamic provisioning.
- **Quotas:** We shouldn't give them unlimited access. We agree on a **ResourceQuota** of 4 vCPUs and 8GB of RAM for the project.
- **Templates:** To help them get started, you point them to the **Developer Catalog** where they can find standard templates for their database and middleware.

---

## Navigation
- [← Back to Section Index]({{ site.baseurl }}/07-storage-templates-catalog/)
- [Next Section: OpenShift Security →]({{ site.baseurl }}/08-openshift-security/)
---
layout: page
title: "OpenShift Installation Methods"
permalink: /03-getting-started-openshift/installation-methods/
---

# OpenShift Installation Methods

OpenShift can be deployed in various environments depending on the use case (development, testing, or production).

## 1. Local Development (Single Node)
- **OpenShift Local (formerly CRC):** Runs a minimal OpenShift cluster on your laptop using a virtual machine.
- **Best for:** Personal learning and offline development.

## 2. Managed Services (Public Cloud)
- **ROSA:** Red Hat OpenShift on AWS.
- **ARO:** Azure Red Hat OpenShift.
- **OpenShift Dedicated:** Managed by Red Hat on Google Cloud or AWS.
- **Best for:** Enterprise production without managing the underlying control plane.

## 3. Self-Managed Clusters
- **Full Installation:** Using the Installer-Provisioned Infrastructure (IPI) or User-Provisioned Infrastructure (UPI) on bare metal, VMware, or cloud.
- **Best for:** Total control over hardware and networking.

## 4. Free Cloud Learning
- **Developer Sandbox:** A free, shared OpenShift cluster provided by Red Hat for 30-day periods.
- **Best for:** Beginners who want to start immediately without installing software locally.

---

## Navigation
- [← Back to Section Index]({{ site.baseurl }}/03-getting-started-openshift/)
- [Next: OpenShift Local (CRC) →]({{ site.baseurl }}/03-getting-started-openshift/openshift-local-crc/)
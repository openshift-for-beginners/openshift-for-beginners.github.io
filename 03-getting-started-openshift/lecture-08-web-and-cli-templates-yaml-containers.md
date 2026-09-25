---
layout: page
title: "Interaction Tools: Web Console and CLI"
permalink: /03-getting-started-openshift/lecture-08-web-and-cli-templates-yaml-containers/
---

# Web Console and CLI Basics

There are two primary ways to manage OpenShift resources.

## 1. OpenShift Web Console
A graphical user interface (GUI) accessed via the browser. 
- **Administrator View:** Focused on nodes, users, storage, and cluster health.
- **Developer View:** Focused on application topology, builds, and monitoring.

## 2. OpenShift CLI (`oc`)
The `oc` tool is a command-line utility used to interact with the cluster API. It is an extension of `kubectl`.

### Essential Commands
- **Login:** `oc login -u <username> -p <password> <server-url>`
- **Check Status:** `oc status`
- **View Projects:** `oc get projects`
- **Apply YAML:** `oc apply -f file.yaml`

### Why use both?
- The **Console** is great for visualizing architecture and finding resources.
- The **CLI** is essential for automation, scripting, and faster troubleshooting.

---

## Navigation
- [← Previous: Developer Sandbox]({{ site.baseurl }}/03-getting-started-openshift/lecture-07-install-single-node-using-sandbox/)
- [Next: UI Overview →]({{ site.baseurl }}/03-getting-started-openshift/lecture-09-openshift-ui-overview/)
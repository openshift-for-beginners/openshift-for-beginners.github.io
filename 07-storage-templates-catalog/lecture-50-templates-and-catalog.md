---
layout: page
title: "Lecture 50: Templates and Catalog"
permalink: /07-storage-templates-catalog/lecture-50-templates-and-catalog/
---

# Lecture 50: Templates and Catalog

### Templates
An OpenShift **Template** is a YAML file that describes a set of objects (Services, Deployments, Routes) that can be parameterized.
- **Parameters:** Allows users to input values like `DB_NAME` or `IMAGE_VERSION` at deployment time.

### Service Catalog
The **Developer Catalog** (in the Web Console) is a collection of these templates. It allows developers to deploy complex stacks (like a "CakePHP + MySQL" app) with a single click by filling out a form.

---

## Navigation
- [← Previous: Lecture 49]({{ site.baseurl }}/07-storage-templates-catalog/lecture-49-demo-deploy-voting-app/)
- [Next Topic: Lecture 51 - Demo Custom Catalog →]({{ site.baseurl }}/07-storage-templates-catalog/lecture-51-demo-custom-catalog/)
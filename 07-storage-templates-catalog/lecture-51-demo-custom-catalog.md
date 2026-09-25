---
layout: page
title: "Lecture 51: Demo - Create a custom Catalog"
permalink: /07-storage-templates-catalog/lecture-51-demo-custom-catalog/
---

# Lecture 51: Demo - Create a custom Catalog

### 1. View Templates
```bash
oc get templates -n openshift
```

### 2. Use a Template via CLI
```bash
oc new-app --template=ruby-helloworld-sample -p NAME=my-app
```

### 3. Customizing the Catalog
By adding your own custom YAML templates to the `openshift` namespace (as an admin), you can make your company's standard application stacks available to all developers in the UI Catalog.

---

## Navigation
- [← Previous: Lecture 50]({{ site.baseurl }}/07-storage-templates-catalog/lecture-50-templates-and-catalog/)
- [Next Topic: Lecture 52 - Quiz →]({{ site.baseurl }}/07-storage-templates-catalog/lecture-52-quiz-storage-templates-catalog/)
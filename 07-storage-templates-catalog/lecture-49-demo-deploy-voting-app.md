---
layout: page
title: "Lecture 49: Demo - Deploy Voting App"
permalink: /07-storage-templates-catalog/lecture-49-demo-deploy-voting-app/
---

# Lecture 49: Demo - Deploy Voting App

### Deployment Strategy
We deploy each component using the `oc new-app` command or by applying YAML files.

### Key Steps
1. Create a project: `oc new-project voting-app`.
2. Deploy the databases (Redis and Postgres).
3. Deploy the application tiers (Voting, Result, and Worker).
4. **Check Persistence:** Verify that the Postgres database has a PVC so votes aren't lost if the pod restarts.
5. **Routes:** Create routes for the `vote` and `result` services to access them from your browser.

---

## Navigation
- [← Previous: Lecture 48]({{ site.baseurl }}/07-storage-templates-catalog/lecture-48-voting-app-introduction/)
- [Next Topic: Lecture 50 - Templates and Catalog →]({{ site.baseurl }}/07-storage-templates-catalog/lecture-50-templates-and-catalog/)
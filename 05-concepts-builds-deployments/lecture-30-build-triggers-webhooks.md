---
layout: page
title: "Lecture 30: Build Triggers, Webhooks, and Image Changes"
permalink: /05-concepts-builds-deployments/lecture-30-build-triggers-webhooks/
---

# Lecture 30: Build Triggers and Webhooks

Automation is what makes OpenShift a true platform. Triggers allow builds to start without manual intervention.

### 1. Webhooks (GitHub / GitLab)
You can configure your Git repository to send a "signal" (Webhook) to OpenShift whenever you push code.
- OpenShift provides a unique URL for each `BuildConfig`.
- You paste this URL into your GitHub/GitLab repository settings.
- **Result:** Code push → Webhook sent → OpenShift starts Build.

### 2. Image Change Trigger
A build can be triggered when its **Base Image** changes. 
- Example: If the official Red Hat Python builder image gets a security patch, your application build can automatically re-run to incorporate that patch.

### 3. Config Change Trigger
A build is triggered immediately when the `BuildConfig` YAML itself is created or modified.

---

## Navigation
- [← Previous: Lecture 29]({{ site.baseurl }}/05-concepts-builds-deployments/lecture-29-custom-build/)
- [Next Topic: Lecture 31 - Quiz →]({{ site.baseurl }}/05-concepts-builds-deployments/lecture-31-quiz-builds-and-deployments/)
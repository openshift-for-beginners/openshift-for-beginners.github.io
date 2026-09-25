---
layout: page
title: "Role Play 2: Troubleshoot a failing S2I build"
permalink: /05-concepts-builds-deployments/role-play-02-troubleshoot-failing-s2i-build/
---

# Role Play 2: Troubleshoot a failing S2I build

### Scenario
A developer in your team is trying to deploy a Node.js application using S2I, but the build status is "Failed".

### Step 1: Investigation
Ask the developer: *"Can you provide the logs for the failed build?"*
- Run: `oc logs build/myapp-1`

### Step 2: Analysis
You see the following error in the logs:
`sh: npm: command not found`

### Step 3: Resolution
Check the `BuildConfig`:
- Run: `oc describe bc myapp`
- **Finding:** The developer accidentally used a **Python** builder image instead of a **Node.js** builder image.
- **Fix:** Update the `BuildConfig` to point to the correct Node.js Image Stream and start the build again (`oc start-build myapp`).

---

## Navigation
- [← Back to Section Index]({{ site.baseurl }}/05-concepts-builds-deployments/)
- [Next Section: Networks, Services, Routes and Scaling →]({{ site.baseurl }}/06-networks-services-routes-scaling/)
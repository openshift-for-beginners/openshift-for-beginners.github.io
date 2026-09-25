---
layout: page
title: "Role Play 2: Troubleshooting S2I Builds"
permalink: /05-concepts-builds-deployments/role-play-02/
---

# Role Play: Troubleshooting an S2I Build

### Scenario
A developer comes to you saying their application build is failing. They are using the Source-to-Image (S2I) strategy.

### Troubleshooting Steps
1. **Check Build Status:** `oc get builds`. Is it "Failed" or "Error"?
2. **Inspect Logs:** `oc logs build/<name>`. Look for compilation errors or missing dependencies.
3. **Check the Image Stream:** Is the builder image (e.g., `python:3.9`) available in the project or cluster?
4. **Webhook Issues:** If the build didn't start at all after a git push, check if the Webhook URL in GitHub matches the one in the `BuildConfig`.

### Result
You discover the developer forgot to include a `requirements.txt` file (for Python) or `package.json` (for Node.js), so the S2I builder image didn't know how to install the dependencies.

---

## Navigation
- [← Previous: Routes Overview]({{ site.baseurl }}/05-concepts-builds-deployments/routes-overview/)
- [Next: Knowledge Check →]({{ site.baseurl }}/05-concepts-builds-deployments/quiz/)
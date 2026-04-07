---
description: >-
  Some Linux users are receiving the "Error adding new nodes. When trying run a
  node, we reached the maximum amount of retries (5)."
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/mHMagc6BlRPNTxTKcyjL/guides/troubleshooting/maximum-amount-of-retries-5-linux
---

# Maximum amount of retries (5) - Linux



<figure><img src="../../.gitbook/assets/image (18).png" alt=""><figcaption></figcaption></figure>

1. Launchpad is designed to create a non-root ant user to manage node processes and store node data under the current user's `~/.local`  If you run as root, the structure gets created under `/root/.local` . The ant user does not have access to that directory, so the nodes cant start&#x20;
2. You must run as root OR add a secondary hard drive or use another directory. Mount it and set permissions so that the ant user can access it. In LP, configure it to use the alternate path for nodes.&#x20;



<br>


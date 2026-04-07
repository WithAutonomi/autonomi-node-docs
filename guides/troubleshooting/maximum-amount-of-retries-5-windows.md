---
description: >-
  Some Window users are receiving the "Error adding new nodes. When trying run a
  node, we reached the maximum amount of retries (5)."
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/mHMagc6BlRPNTxTKcyjL/guides/troubleshooting/maximum-amount-of-retries-5-windows
---

# Maximum amount of retries (5) - Windows



<figure><img src="../../.gitbook/assets/image (18).png" alt=""><figcaption></figcaption></figure>

1. To solve this, hit the Windows key and search for "services.msc" and click it&#x20;
2. Scroll down to "antnode"&#x20;

<figure><img src="../../.gitbook/assets/image (33).png" alt=""><figcaption></figcaption></figure>

3. Now hit the Windows key and type "CMD", and right click it to "Run as Administrator"
4. Type in CMD: "sc delete antnode1" (Note: you may need to do "sc delete safenode1" as well)
5. Do this for all the services you see in **Step 2**
6. Relaunch LP, reset your nodes, and start them back up.&#x20;


---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/mHMagc6BlRPNTxTKcyjL/guides/troubleshooting/the-number-of-services-to-add-does-not-match-the-number-of-ports
---

# The number of services to add does not match the number of ports

This is a common error many CLI users face, it is an easy fix. In the below instance, the user wanted to open 40 ports, but accidently opened 41 ports. Adjust the range from 45000-45040 to 45000-45039. &#x20;

<figure><img src="../../.gitbook/assets/image (11).png" alt=""><figcaption></figcaption></figure>

---
description: >-
  Some Windows users experience Launchpad crashing a second after launching it.
  But have no fear, we have a fix for you!
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/mHMagc6BlRPNTxTKcyjL/guides/troubleshooting/launchpad-crashes-right-away-windows
---

# Launchpad crashes right away -  Windows

{% hint style="danger" %}
If you can not locate some of these folders please make sure they are [not hidden](../how-to-guides/view-hidden-files.md).
{% endhint %}

1. Delete the "safe" and "autonomi" folders found at:

`C:\Users\YOURCOMPUTERNAME\AppData\Roaming\safe`

`C:\Users\YOURCOMPUTERNAME\AppData\Roaming\autonomi`

<figure><img src="../../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>

2. Delete the following folders found at:

`C:\ProgramData\safenode`

`C:\ProgramData\safenode-manager`

`C:\ProgramData\antnode`

`C:\ProgramData\antctl`

`C:\ProgramData\service-manager`

<figure><img src="../../.gitbook/assets/image (30).png" alt=""><figcaption></figcaption></figure>

3. Reinstall [Launchpad](https://docs.autonomi.com/getting-started/downloads) and run it as a administrator




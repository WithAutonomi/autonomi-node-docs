---
description: >-
  If you want to check if your nodes are having connection issues, preventing
  them from earning, here's what you can do…
hidden: true
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/mHMagc6BlRPNTxTKcyjL/guides/troubleshooting/checking-your-connection-from-a-home-network
---

# Checking your connection from a Home Network

1. [**Reset your nodes**](../how-to-guides/reset-your-nodes.md) and then start them again
2. **Let them run** for several minutes
3. [**Open the log file**](../how-to-guides/access-the-logs.md) of a node
4. **Search the file** for the phrase `HandshakeTimedOut` and/or `CircuitReqDenied`.

Some of these errors can be expected in a typical log, but if you're finding them in large numbers (e.g. >1000) then this indicates that your nodes are struggling to make connections from behind your router.

### Fixes and Improvements on the way

We are working on improvements and optimisations that should significantly improve and mitigate this issue, if not eliminate it altogether. So keep an eye out for updates! We'll ask you to reset your nodes when they are ready.

### Other Solutions

If you are comfortable with getting your hands a bit more dirty and are happy to tinker other more short-term solutions might be to:

* Use the [Node CLI](../how-to-guides/use-the-node-cli.md), which offers more configuration options and may help get things going
* Use an aftermarket router which allows advanced configuration, such as port forwarding.

The best place to start is by asking our friendly community for help, either over on the [forum](https://forum.autonomi.community) or on [Discord](https://discord.gg/autonomi).

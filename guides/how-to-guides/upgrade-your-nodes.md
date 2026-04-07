---
description: >-
  Upgrades to the Network are made periodically. There's a simple procedure to
  follow when an update is announced and you are asked to upgrade your nodes to
  the latest version
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/mHMagc6BlRPNTxTKcyjL/guides/how-to-guides/upgrade-your-nodes
---

# Upgrade Your Nodes

## Upgrade using the Node Launchpad

{% stepper %}
{% step %}
Make sure you have the [Latest Launchpad](../../downloads.md), and open it.
{% endstep %}

{% step %}
**Press O** to open the Options Screen
{% endstep %}

{% step %}
Press **Ctrl + U** and then **Enter** to begin the upgrade

_Upgrading can take several minutes for each node. Please don't close the app or stop your nodes during this process._
{% endstep %}

{% step %}
Your nodes will then stop&#x20;

_Notice they have been upgraded to the latest version_
{% endstep %}

{% step %}
Start your nodes again by pressing **Ctrl + S**
{% endstep %}
{% endstepper %}

## Upgrading using the CLI

If you are using the [Node CLI](use-the-node-cli.md), your nodes will update themselves automatically over time, so you do not need to manually reinstall the node binary for normal updates.

```bash
ant update
```

If you want to update the `ant` CLI itself, run the command above.

If you are setting up nodes from the CLI for the first time, start with [Use the Node CLI](use-the-node-cli.md).

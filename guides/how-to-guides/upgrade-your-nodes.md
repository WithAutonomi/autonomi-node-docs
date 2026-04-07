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

If you are a power user utilizing our [Node Manager](https://github.com/maidsafe/autonomi/tree/main/ant-node-manager) CLI tool and want to upgrade your nodes to the latest version, first make sure you have the latest version of the Node Manger with the command:

```bash
antup update
```

Then, to begin upgrading your nodes, use the command:

```bash
antctl upgrade --interval 60000
```

Using the `--interval 60000` argument will leave 60 seconds pause between upgrading each of your nodes. This is recommended for people running up to 50 nodes.&#x20;

If you are running more than 50 nodes we'd recommend a longer interval of `90000` or more.

{% hint style="warning" %}
Once upgraded run the command **`antctl start --interval 60000`**&#x20;
{% endhint %}

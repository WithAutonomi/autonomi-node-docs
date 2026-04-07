---
description: >-
  Here's how to use the ant CLI to run one or more Autonomi nodes from your
  terminal and contribute storage space to the Network
---

# Use the Node CLI

The `ant` CLI lets you run one or more Autonomi nodes from your terminal and contribute your spare storage space to the Network.

{% hint style="info" %}
If this is your first time, we'd recommend you start with just a single node, so you can get a feel for how your machine and connection handle it. Then add more as your resources allow.
{% endhint %}

{% hint style="info" %}
You only need your public wallet address for this. Do not paste your private key or secret recovery phrase into any of these commands.
{% endhint %}

{% stepper %}
{% step %}
#### Install the `ant` CLI

On Mac and Linux:

```bash
curl -fsSL https://raw.githubusercontent.com/WithAutonomi/ant-client/main/install.sh | bash
```

On Windows:

```powershell
irm https://raw.githubusercontent.com/WithAutonomi/ant-client/main/install.ps1 | iex
```

When the install finishes, you can check it worked with:

```bash
ant --help
```

If your terminal says `ant` cannot be found, close it and open a new one, then try again.
{% endstep %}

{% step %}
#### Start the background daemon

Run:

```bash
ant node daemon start
```

This starts a small background process that manages your nodes for you.

You can check it is running with:

```bash
ant node daemon status
```
{% endstep %}

{% step %}
#### Add your wallet address

Now register a node with your wallet address:

```bash
ant node add --rewards-address 0xYourWalletAddress
```

Any Ethereum address can be used here, but you'll need a compatible wallet if you want to see and use anything your nodes earn.

If this is the first time you've done this, the CLI will fetch the latest `ant-node` binary for you automatically.
{% endstep %}

{% step %}
#### Start your node

Run:

```bash
ant node start
```

If you only want to start one specific node later on, use its service name instead:

```bash
ant node start --service-name node1
```
{% endstep %}

{% step %}
#### Check that your node is running

To see all of your registered nodes and their status, run:

```bash
ant node status
```

To see a summary of the background daemon, run:

```bash
ant node daemon status
```

The daemon status command will also show you a local console URL you can open in your browser.

Once your node is running, it will begin gathering data and serving it to the Network.

Your nodes will update themselves automatically over time, so you do not need to manually reinstall the node binary for normal updates.
{% endstep %}

{% step %}
#### Add more nodes later if you want to

When you're ready to contribute more storage space, just add more nodes and start them:

```bash
ant node add --rewards-address 0xYourWalletAddress --count 2
ant node start
```

If you'd prefer to choose the ports yourself, you can do that too:

```bash
ant node add --rewards-address 0xYourWalletAddress --count 2 --node-port 12000-12001
```
{% endstep %}

{% step %}
#### Stop your nodes

To stop all of your running nodes, run:

```bash
ant node stop
```

Or stop just one of them:

```bash
ant node stop --service-name node1
```
{% endstep %}

{% step %}
#### Reset everything if you need a clean start

First stop your nodes:

```bash
ant node stop
```

Then reset everything:

```bash
ant node reset --force
```

The reset command will not run while nodes are still running.

This removes your node data, logs, and local node registry, so only use it if you really want to start over.
{% endstep %}

{% step %}
#### Congratulations

You are up and running, and contributing to the Autonomi Network from the Command Line.
{% endstep %}
{% endstepper %}

## Notes

* If you install `ant` using the commands above, you should not need to enter bootstrap peers manually for normal live-network use.
* When you add nodes, the CLI will show you where each node's data and logs are being stored.

## Other useful commands

If you want to stop the background daemon itself, first stop your nodes:

```bash
ant node stop
ant node daemon stop
```

If you want to check the daemon again later:

```bash
ant node daemon status
```

If you want to update the `ant` CLI itself:

```bash
ant update
```

## Advanced options

When adding nodes, there are a few extra options you may find useful:

* `--metrics-port` to set metrics ports
* `--network-id` to target a specific network
* `--bootstrap` to provide bootstrap peers manually
* `--env` to pass environment variables to the node

For a fuller list of commands and options, run:

```bash
ant node --help
ant node add --help
ant node daemon --help
```

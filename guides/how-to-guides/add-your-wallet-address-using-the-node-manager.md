---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/mHMagc6BlRPNTxTKcyjL/guides/how-to-guides/add-your-wallet-address-using-the-node-manager
---

# Add your Wallet Address using the CLI

When adding nodes using the Node CLI, you must specify an [Ethereum Wallet](../../system-requirements.md#compatible-wallets) address to receive anything your nodes earn.

For the full setup flow, see [Use the Node CLI](use-the-node-cli.md).

### Here's how to add your wallet…

```bash
ant node add --rewards-address 0xYourWalletAddress
```

If you want to add more than one node at the same time:

```bash
ant node add --rewards-address 0xYourWalletAddress --count 2
```

### Other useful arguments

When adding nodes, you can also set your own ports or custom data and log locations:

```bash
ant node add \
  --rewards-address 0xYourWalletAddress \
  --count 2 \
  --node-port 12000-12001 \
  --data-dir-path /path/to/data \
  --log-dir-path /path/to/logs
```

{% hint style="info" %}
You only need your public wallet address here. Do not paste your private key or secret recovery phrase into the CLI.
{% endhint %}

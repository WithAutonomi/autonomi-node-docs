---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/mHMagc6BlRPNTxTKcyjL/guides/how-to-guides/add-your-wallet-address-using-the-node-manager
---

# Add your Wallet Address using the Node Manager

When adding nodes using the Node Manager CLI tool, you must specify an [Ethereum Wallet](../../system-requirements.md#compatible-wallets) Address to receive the tokens your node earns, along with the Atbitrum one Network.

### Here's how to add your wallet…

```bash
antctl add <as before> --rewards-address <wallet address> evm-arbitrum-one
```

{% hint style="warning" %}
**`evm-arbitrum-one` must be added at the end**. This is the blockchain Autonomi uses for data rewards and payments.
{% endhint %}

### Full list of arguments

As a reminder, here's the full list of args your can include when adding nodes:

```bash
antctl add (with the following args)
  --count <# of nodes>      => If not specified, only a single node is added
  --rewards-address <your ethereum wallet address> evm-arbitrum-sepolia => Must be specified to store your earned attos. Note: this is also the address where your rewards will be paid after the TGE in after January 2025.
  --data-dir-path <path>    => optional, if you have a second hard disk where you want to store the data to.
  --log-dir-path <path>     => optional, path to store the log files.
  --home-network            => optional, if you're behind a NAT/home router/without port forwarding
  --upnp                    => optional, if you have enabled upnp in your router, mutually exclusive with home-network
  --node-port <single/range of ports> => If --home-network or --upnp is not provided, then you have to portforward a set of ports and provide them here. We accept a single port i.e., 12000 or a range i.e., 12000-12010. The number of ports here should match the number of nodes speicified using --count
  --enable-metrics-server   => optional, if you want the stats to be displayed inside the launchpad
```

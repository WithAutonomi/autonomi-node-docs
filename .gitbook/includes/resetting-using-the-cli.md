---
title: Resetting using the CLI
---

## Resetting using the CLI <a href="#if-you-are-a-node-manager-cli-user-2" id="if-you-are-a-node-manager-cli-user-2"></a>

Here's the series of commands for advanced users already using the Node Manager CLI tool: `antctl`.\
\
After resetting, and while adding nodes again, note the additional arguments that should be used each time depending, on your circumstances. In particular the `--rewards-address` argument which allows you to attach your [wallet](/broken/pages/toNOJmbb6CI5SpEvThmb) address to each node. This is now using the Arbitum One network:

```bash
1. antup update (to make sure you are on the latest version of the Node Manager)
2. antctl reset
3. antctl add (with the following args)
  --count <# of nodes>                                              => If not specified, only a single node is added
   --log-dir-path <path>                                             => optional, path to store the log files.
  --home-network                                                    => optional, if you're behind a NAT/home router/ without port-forwarding
  --upnp                                                            => optional, if you have enabled upnp in your router, mutually exclusive with home-network
  --node-port <single/range of ports>                               => If --home-network or --upnp is not provided, then you have to port-forward a set of ports and provide them here. We accept a single port i.e., 12000 or a range i.e., 12000-12010. The number of ports here should match the number of nodes specified using --count
  --enable-metrics-server                                           => optional, if you want the stats to be displayed inside the launchpad
  --rewards-address <your ethereum wallet address> evm-arbitrum-one => Must be specified at the end, to store your earned ANT.
4. antctl start --interval 2000
5. antctl status --details
```

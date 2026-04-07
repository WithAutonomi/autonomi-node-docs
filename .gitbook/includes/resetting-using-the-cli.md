---
title: Resetting using the CLI
---

## Resetting using the CLI <a href="#if-you-are-a-cli-user" id="if-you-are-a-cli-user"></a>

If you are using the Node CLI, here is the basic reset flow. For the full setup process, see [Use the Node CLI](../../guides/how-to-guides/use-the-node-cli.md).

```bash
ant node daemon start
ant node stop
ant node reset --force
ant node add --rewards-address 0xYourWalletAddress
ant node start
ant node status
```

If you are adding multiple nodes again, include any other arguments you need when you run `ant node add`, such as `--count`, `--node-port`, `--data-dir-path`, or `--log-dir-path`.

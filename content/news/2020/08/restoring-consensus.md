---
title: "Restoring Consensus"
date: 2020-08-10T15:25:29+03:00
draft: false
---

We have 69M STG actively staked. More than 2/3 of the 80+ active nodes seem to have been shut down without the stake being retired first. This means we lost consensus and the blockchain cannot operate. 

Please bring your node back online by shutting it down if it’s already running or just restarting it as usual, e.g. using `stegosd -n mainnet`.

Please use the command-line interface to check if your node started properly by running `stages` and then typing `show status` at the prompt. You should see something like this:

```
Stegos CLI 1.2.245 (66be84cc 2020-08-07)
Type 'help' to get help

account#1> show status
---
- type: status_info
...

---
- type: status_info
  is_synchronized: false
  epoch: 35338
  offset: 50
  view_change: 0
  last_block_hash: 66409d3e2db9a4fa714b5609e7934e0fabb54722a1a5ed038f7e57bd6fa3eb95
  last_mblock_hash: 69699ae0dcf97a577ebaf56832e6ae486d8e78a0b5f6324e13cc05bac9d6c876
  last_mblock_timestamp: "2020-08-05T08:26:13.201143000Z"
  local_timestamp: "2020-08-10T11:41:03.661871000Z"
...
```

If your CLI seems to be stuck then kill the node you are running and prepare a config file with the following 2 lines:

```
[network]
readiness_threshold=0
```

It doesn’t matter where the file is or what it’s named but I will assume it’s `stages.toml`. Once the file is ready, start the node using `stegosd -n mainnet -c stegos.toml` and you should be up and running!

Last but not least, you should see a number of nodes connected to yours. Check for this by typing `show replication` in the CLI. The output should look something like this:

```
account#1> show replication
---
- type: replication_info
...

---
- type: replication_info
  peers:
    - state: discovered
      peer_id: QmPGpgAZvkcnhrYyegvQdSAVMbS3KrtMgvRZsPgyULD1zH
      multiaddr: /ip4/47.75.191.4/tcp/53470
      idle: 38m 6s 936ms 16us 711ns
    - state: discovered
      peer_id: QmbHx9fotuPLbejjpdEQHmBzUio6MGZW4uQsW9EQCH1PJD
      multiaddr: /ip4/207.180.225.152/tcp/41580
      idle: 5m 55s 215ms 32us 640ns
    - state: discovered
      peer_id: QmP3JxeHdRUK9QmYPk2RpCpk4hNazyUWtnmhRpdSX4ogi1
      multiaddr: /ip4/207.180.225.152/tcp/41854
      idle: 1m 51s 659ms 256us 974ns
    - state: discovered
      peer_id: QmdgvHUnNZ6Q9abD1B6x3cLbzFXVgKBFpXNBConLznm4ie
      multiaddr: /ip4/49.235.181.188/tcp/56740
      idle: 34m 36s 934ms 717us 648ns
    - state: discovered
      peer_id: Qmdcm7VsrsDV6s46Jm6cCEHCuFRtYLoxeWv1ZYX6BCKqrY
      multiaddr: /ip4/207.180.225.152/tcp/41590
      idle: 5m 54s 403ms 620us 591ns
...
```


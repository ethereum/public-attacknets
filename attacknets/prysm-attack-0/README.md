# `prysm-attack-0` (`beta-0`)

***STATUS***: _active_

This directory contains the client configuration info and files for an
all prysm `v0.12.1` attacknet composed of 4 nodes and 128 validators.

## Configuration

- Spec version: `v0.12.1`
- Genesis Time: `1595202934` (07/19/2020 @ 11:55:34pm (UTC))
- Genesis Fork Version: `0x00000000`
- Fork Digest: `c354a54a`
- Initial State Root: `0xc9d4754d298779a097fb46855d49ee1fd2ad33642e6ee9540f37810fa97ebd7b`
- Genesis Block Root: `0x2bdde8c274a94784b376fbef30bc946fc417550a22c0ac9cb10b8d93d27cad1b`
- Deposit Contract: [`0x0d9D6D3Aa0791D3B3F4f489b46dCD2586C1011C4`](https://goerli.etherscan.io/address/"0x0d9D6D3Aa0791D3B3F4f489b46dCD2586C1011C4) ([Goerli Testnet](https://github.com/goerli/testnet))
- Deposit Contract Deploy Block Hash: `0x9402554e798e2f0e2974ac68961130bc069fb58231bd7c8fa361f24245407550`
- Deposit Contract Deploy Block Number: `0x9402554e798e2f0e2974ac68961130bc069fb58231bd7c8fa361f24245407550`
- `MIN_GENESIS_TIME`: `1578009600`
- `MIN_GENESIS_ACTIVE_VALIDATOR_COUNT`: `128`
- `GENESIS_DELAY`: `1000`
- Chain Explorers: None
- Status Dashboard: None

## Rules

Please see [general attacknet rules](../../README.md#general-rules) in addition
to the following:

* **The goal**: _prevent finality on a single network for 16 continuous epochs_
* **The rules**:
    * _By any means necessary_. Seriously.
      The scope of these initial networks is purposefully wide open to encourage
      participation and experimentation. In subsequent nets, we might have more scoped out
      challenges and rules, but for _`beta-0_, let's just dig in.
    * _Show your work_. To qualify for the reward, you must (1) point specifically to the epoch range that affected,
      (2) provide some sort of proof that you caused the outage,
      and (3) provide technical details about the attack and how it was performed.
* **The reward**: _**$5k (USD)** for each net to the first entity to achieve the goal._
  Maximum one reward per entity for `beta-0` attacknets. If you take down `lighthouse-attack-0`,
  you do not qualify for the reward for `prysm-attack-0` and vice versa.
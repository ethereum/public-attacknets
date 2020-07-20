# `lighthouse-attack-0` (`beta_0`)

***STATUS***: _active_

## Configuration

This directory contains the client configuration info and files for an
all lighthouse `v0.12.1` attacknet composed of 4 nodes and 128 validators.

- Spec version: `v0.12.1`
- Genesis Time: `1595211161` (07/20/2020 @ 2:12:41am (UTC))
- Genesis Fork Version: `0x00000000`
- Fork Digest: `80e1769b`
- Initial State Root: `0x9fc01c541de1bb13531c40f4f24c4c378cf03addc6cae4f05fc856fbd39b22a8`
- Genesis Block Root: `0x075fe0f11955d08ea1d29b60ef5623b9b226133aed31b50bd49c304454e53485`
- Deposit Contract: [`0xdbb44f3e33640A820eECc0b893ED5aEC17150dbf`](https://goerli.etherscan.io/address/0xdbb44f3e33640A820eECc0b893ED5aEC17150dbf) ([Goerli Testnet](https://github.com/goerli/testnet))
- Deposit Contract Deploy Block Hash: `0x2592432bba5f7850a9afb52cc08e1c3ef2da885c6fea0e936ee51810b2f955fe`
- Deposit Contract Deploy Block Number: `3076609`
- `MIN_GENESIS_TIME`: `1578009600`
- `MIN_GENESIS_ACTIVE_VALIDATOR_COUNT`: `128`
- `GENESIS_DELAY`: `300`
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
      challenges and rules, but for _`beta_0`_, let's just dig in.
    * _Show your work_. To qualify for the reward, you must (1) point specifically to the epoch range that affected,
      (2) provide some sort of proof that you caused the outage,
      and (3) provide technical details about the attack and how it was performed.
* **The reward**: _**$5k (USD)** to the first entity to achieve the goal._
  Maximum one reward per entity for `beta_0` attacknets. If you take down `lighthouse-attack-0`,
  you do not qualify for the reward for `prysm-attack-0` and vice versa.
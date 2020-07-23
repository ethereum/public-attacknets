# `teku-attack-0` (`beta-0`)

***STATUS***: _active_

This directory contains the client configuration info and files for an
all teku `v0.12.1` attacknet composed of 4 nodes and 128 validators.

## Configuration

- Spec version: `v0.12.1`
- Genesis Time: `1595463896`
- Genesis Fork Version: `0x00000000`
- Fork Digest: `157d3034`
- Initial State Root: `0x7dc34e412319ccb338120908f5a08b9588e1270ee47130d005cb227dd3ea8bf5`
- Genesis Block Root: `0x97b4dc23023e7c29bd3e129ea3b53f15e26eb495982461f267751485d957839d`
- Deposit Contract: [`0x99573b94Fd4Fc0ea48AC63A5a78738Fd430f1aFc`](https://goerli.etherscan.io/address/0x99573b94Fd4Fc0ea48AC63A5a78738Fd430f1aFc) ([Goerli Testnet](https://github.com/goerli/testnet))
- Deposit Contract Deploy Block Hash: `0x2a255181db76aa902acc31e87205a3899d24090d30bbae0ce25496036e99d8e5`
- Deposit Contract Deploy Block Number: `3093724`
- `MIN_GENESIS_TIME`: `1578009600`
- `MIN_GENESIS_ACTIVE_VALIDATOR_COUNT`: `128`
- `GENESIS_DELAY`: `300`
- Bootnode ENR(s):
  - `enr:-KG4QLbHkqa5d6Ap0bBEuLUazyWPVbdVsZ_Py-9zFH0Uh9NMS9V-gzEvRzyMV0kPv1vsQafu1hZu8c3jDEdxn0INEnwDhGV0aDKQFX0wNAAAAAD__________4JpZIJ2NIJpcIQNciWwiXNlY3AyNTZrMaEC398ggkQb5G2M8QuLva2CCMqe9mFGQyb0SEM6_MDiGdiDdGNwgiMog3VkcIIjKA`
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
* **The reward**: _**$5k (USD)** to the first entity to achieve the goal._
  Maximum one reward per entity for `beta-0` attacknets. If you take down `lighthouse-attack-0`,
  you do not qualify for the reward for `prysm-attack-0` and vice versa.
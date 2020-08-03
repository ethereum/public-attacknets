# `mc-attack-0` (`beta_1`)

***STATUS***: _active_

## Configuration

This directory contains the client configuration info and files for a
multi-client `v0.12.1` attacknet composed of 15 nodes and 4500 total validators, split
across three clients (prysm, lighthouse, and teku).

- Spec version: `v0.12.2`
- Genesis Time: `1596327220` (2020/08/02 @ 12:13am (UTC))
- Genesis Fork Version: `0x0000b01d`
- Fork Digest: `2e44918e`
- Initial State Root: `0xf2a928a4fc6e63c3ad520ec7340b646aa3772991727cf0eeb0dd0a5f6c644e25`
- Genesis Block Root: `0xed8e76a43a622ff116992d8c9cca44981c840d424391870c5302a22e0ae5ebcc`
- Deposit Contract: [`0x38c750cFFb382cDD3644C40A39540a9b4b46b0cf`](https://goerli.etherscan.io/address/0x38c750cFFb382cDD3644C40A39540a9b4b46b0cf) (_Note_ this is a modified deposit contract with access control features. See [`beta-1`](../README.md#attacker-validators) rules for more details on registering validators)
- Deposit Contract Deploy Block Hash: `0x7459ad12e5dfe0e513ea1a5fef498c54f268d654f721df56e0e2fe5012e13998`
- Deposit Contract Deploy Block Number: `3150443`
- `MIN_GENESIS_TIME`: `1578009600`
- `MIN_GENESIS_ACTIVE_VALIDATOR_COUNT`: `4500`
- `GENESIS_DELAY`: `900`
- Bootnode ENR(s):
  - `enr:-LK4QC4pexs3ghjGOItTkTttDiow--WuQqjtieE0YRVKxnvHWAUjt2GKH8-WRDoj8ZSOIBJodAWG-ZftKOPwqTK8QtxBh2F0dG5ldHOI__________-EZXRoMpAuRJGOAACwHf__________gmlkgnY0gmlwhDZBuWeJc2VjcDI1NmsxoQOuTMWhnh6C8oEcCNEyLueXHOJD4zsZr06rGRFC-pbDzIN0Y3CCIyiDdWRwgiMo`
  - `enr:-LK4QGaMPlU00DocKfM4ciAnzn44SWYfDNw0Vk2nVj8Uv7r8KEhO_wqbHzEWAzBpjuQLBIwXj91sQCHFR_kDMglcf4IGh2F0dG5ldHOI__________-EZXRoMpAuRJGOAACwHf__________gmlkgnY0gmlwhDRBowiJc2VjcDI1NmsxoQLNz5fvAiF0KiVdV9YU_AucPRlA9vtgaCfpxpiA9MSrB4N0Y3CCIyiDdWRwgiMo`
  - `enr:-LK4QKT94GydM4k0rV9LNIQn3vGwn8qO8Osh-3wSV970M241IT7hCG17Vzv5fiMAJ95b4v6Pkp814X0OAc-SWzM7pnAEh2F0dG5ldHOI__________-EZXRoMpAuRJGOAACwHf__________gmlkgnY0gmlwhAMZfQmJc2VjcDI1NmsxoQKVusiPi55UDoIJS6R0A_wiygNr4ZK-vbYWwoJ6Fbb4E4N0Y3CCIyiDdWRwgiMo`
- Chain Explorers: None
- Status Dashboard: [attacknet.eth2.wtf](https://attacknet.eth2.wtf)

## Rules

Please see [beta-1 rules](../README.md#rules) and [general attacknet rules](../../../README.md#general-rules).
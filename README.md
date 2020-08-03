# Public eth2 attacknets

This repository tracks public "attacknets" maintained by the EF.

## Multi-client `beta-1` attacknet

A multi-client [beta-1 attacknet](./attacknets/beta-1) composed of three
clients is up with multiple tiers of bounties (up to $15k!). [Read more](./attacknets/beta-1)
for details about configuration, rules, and rewards.

## Single-client `beta-0` attacknets

Single-client [beta-0 attacknets](./attacknets/beta-0) remain up, each with a continuous $5k bounty
for novel exploits leading to sustained loss of finality.

_Each network has a possible reward of $5k!_ [Read more](./attacknets/beta-0)
for details about configuration, rules, and rewards.

Deposits are not enabled in `beta-0` testnets so you'll have to try
non-validator based attacks for this run.

See README for each net for network configuration and rules/rewards.

## Attacknet directory structure

Each attacknet is contained within it's own sub-directory within [`./attacknets`](./attacknets).

Within the attacknet directory, a `README.md` is provided with human
readable, high-level configuration as well as the rules and any rewards
associated with the attacknet.

The attacknet directory also provides configuration files that might be useful
in running clients and connecting to the network.

* `prysm_config.yaml` -- is a YAML configuration file that can be ingested by
  the Prysm client via the `--chain-config-file` commandline flag
* `teku_config.yaml` -- is a YAML configuration file that can be ingested by
  the Teku client via the `--network` commandline flag
* `lighthouse` -- is the testnet configuration directory that can be
  ingested by the Lighthouse client via the `--testnet-dir` commandline flag

## General rules

In addition to attacknet specific rules provided for in each attacknet. The
following are the general rules for the program. [_Note_: This program is in `beta-0`
and all rules are subject to change without prior notice].

* The Ethereum Foundation is solely responsible for judging the attack and deciding on rewards
* The Ethereum Foundation _may_ reward "honorable mention" rewards of any
  denomination for interesting effects induced on testnets that do not
  necessarily meet the stated goal
* Awards can be redeemed in ETH or DAI
* Eth2 client teams are eligible to participate only on attacknets that do not contain their specific client

### How to report

All claims on attacknet rewards must be reported as an issue in this repo.

Please follow this reporting structure to aid in prompt review:

* If succeeded in a testnet goal and want to make a claim on the reward, prefix the name of the Issue/PR with "[`{ATTACK_NET_NAME}` Reward]"
  Use [this template](https://github.com/ethereum/public-attacknets/issues/new?assignees=&labels=&template=attacknet-reward.md&title=%5BATTACKNET_NAME+Reward%5D)
  for convenience.
* If want to share something interesting achieved outside of the goal, prefix the name of the Issue/PR with "[`{ATTACK_NET_NAME}` Issue]"
  Use [this template](https://github.com/ethereum/public-attacknets/issues/new?assignees=&labels=&template=attacknet-issue.md&title=%5BATTACKNET_NAME+Issue%5D)
  for convenience.
* Use the following structure for the body of the Issue/PR

    * **Description**: _High-level description of the attack [1 sentence]_

    * **Attack scenario**: _More detailed description of the attack scenario and how it was carried out [1 to 3 sentences]_

    * **Impact**: _Describe the effect had on the attacknet [1 to 2 sentences]_

    * **Details**: _Very specific details about the attack including the specific slots/epochs where it can be observed_

### Privacy

The Ethereum Foundation is not responsible for any private information that might
be leaked as a result of this program.

In the event that the reporting of an attack _does leak_ private information
(e.g. logs from a testnet containing IP addresses), we ask that you withhold any such information in the public report.
Instead, please note that there are additional accompanying resources to be shared,
and the attacknet evaluators will be in touch.

### Important legal information

We give explicit permission to attack these attacknets over the internet.

This attacknet program is an experimental and discretionary rewards program for
our active Ethereum community to encourage and reward those who are helping
to improve the platform. It is not a competition. You should know that we can
cancel the program at any time, and rewards are at the sole discretion of Ethereum Foundation.
In addition, we are not able to issue rewards to individuals who are on sanctions
lists or who are in countries on sanctions lists (e.g. North Korea, Iran, etc).
You are responsible for all taxes. All rewards are subject to applicable law.
Finally, your testing must not violate any law or compromise any data that is not yours.

## Getting started

### Running clients with custom config files

For each attacknet, a README.md and configuration files are provided to allow
for easy running of clients. Note that a `prysm_config.yaml`, `teku_config.yaml`, and `lighthouse` directory
are provided for each testnet regardless of the constituent clients making up
the testnet. These are configuration files that you can use to run lighthouse,
prysm, and/or teku on each testnet.

To run [lighthouse](https://github.com/sigp/lighthouse/), in addition to normal
configuration commandline flags, use the following:
* `--testnet-dir {LIGHTHOUSE_TESTNET_DIR}` where `LIGHTHOUSE_TESTNET_DIR`
  is the `lighthouse` directory found within the specific attacknet

To run [prysm](https://github.com/prysmaticlabs/prysm/), in addition to normal
configuration commandline flags, use the following:
* `--chain-config-file {PRYSM_CONFIG_FILE}` where `PRYSM_CONFIG_FILE` is the
  `prysm_config.yaml` file found within the specific attacknet
* `--deposit-contract {DEPOSIT_CONTRACT_ADDR}` where `DEPOSIT_CONTRACT_ADDR` is
  the `0x` prefixed deposit contract address found in the specific attacknet
  README.md
* `--contract-deployment-block {DEPOSIT_CONTRACT_DEPLOY_NUMBER}` where `DEPOSIT_CONTRACT_DEPLOY_NUMBER` is
  the block number at which the deposit contract was deployed, found in the attacknet README.md
* `--custom-genesis-delay {GENESIS_DELAY}` where `GENESIS_DELAY` is
  the genesis delay param found in the attacknet README.md

To run [teku](https://github.com/pegasyseng/teku), in addition to normal configuration
commandline flags, use the following:
* `--network {TEKU_CONFIG_FILE}` where `TEKU_CONFIG_FILE` is the
  `teku_config.yaml` file found within the specific attacknet
* `--eth1-deposit-contract-address {DEPOSIT_CONTRACT_ADDR}` where `DEPOSIT_CONTRACT_ADDR` is
  the `0x` prefixed deposit contract address found in the specific attacknet
  README.md


### Rumor -- Eth2 interactive shell

@protolambda maintains [`rumor`](https://github.com/protolambda/rumor),
an eth2 interactive shell for dynamically interacting with eth2 networks and data.

Check out the rumor [README](https://github.com/protolambda/rumor) for basic
documentation. We expect this tool to be invaluable in getting started,
understanding networks, and constructing attacks.



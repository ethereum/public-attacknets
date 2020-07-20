# Public eth2 attacknets

This repository tracks public "attacknets" maintained by the EF.

## Beta 0

This program is currently in "beta-0" and all details are subject to change

Active beta-0 attacknets:
* [`lighthouse-attack-0`](./attacknets/lighthouse-attack-0)
* [`prysm-attack-0`](./attacknets/prysm-attack-0)

`lighthouse-attack-0` and `prysm-attack-0` are real networks, ready for you to attack,
but they are beta in the sense that it's our first go at this -- we expect to learn and iterate quickly.
These networks are also very small (only 4 nodes each!) so should be pretty easy to take down.

Deposits are not enabled in `beta-0` testnets so you'll have to try
non-validator based attacks for this run.

See README for each net for network configuration and rules/rewards.

View [original announcement](https://notes.ethereum.org/@djrtwo/attacknets-beta-0).

## Attacknet directory structure

Each attacknet is contained within it's own sub-directory within [`./attacknets`](./attacknets).

Within the attacknet directory, a `README.md` is provided with human
readable, high-level configuration as well as the rules and any rewards
associated with the attacknet.

The attacknet directory also provides configuration files that might be useful
in running clients and connecting to the network.

* `prysm_config.yaml` -- is a YAML configuration file that can be ingested by
  the Prysm client via the `--chain-config-file` commandline flag
* `lighthouse-testnet` -- is the testnet configuration directory that can be
  ingested by the Lighthouse client via the `--testnet-dir` commandline flag

## General rules

In addition to attacknet specific rules provided for in each attacknet. The
following are the general rules for the program. [_Note_: This program is in `beta-0`
and all rules are subject to change without prior notice].

* The Ethereum Foundation is solely responsible for judging the attack and deciding on rewards
* Awards can be redeemed in ETH or DAI
* Eth2 client teams are eligible to participate only on attacknets that do not contain their specific client

## How to report

All claims on attacknet rewards must be reported as an issue in this repo.

Please follow this reporting structure to aid in prompt review:

* Prefix the name of the Issue/PR with "[{ATTACK\_NET\_NAME} Reward]
* Use the following structure for the body of the Issue/PR

    * **Description**: _High-level description of the attack [1 sentence]_

    * **Attack scenario**: _More detailed description of the attack scenario and how it was carried out [1 to 3 sentences]_

    * **Impact**: _Describe the effect had on the attacknet [1 to 2 sentences]_

    * **Details**: _Very specific details about the attack including the specific slots/epochs where it can be observed_

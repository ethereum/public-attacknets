# Public eth2 attacknets

This repository tracks public "attacknets" maintained by the EF.

## `beta-0`

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

### How to report

All claims on attacknet rewards must be reported as an issue in this repo.

Please follow this reporting structure to aid in prompt review:

* Prefix the name of the Issue/PR with "[{ATTACK\_NET\_NAME} Reward]
* Use the following structure for the body of the Issue/PR

    * **Description**: _High-level description of the attack [1 sentence]_

    * **Attack scenario**: _More detailed description of the attack scenario and how it was carried out [1 to 3 sentences]_

    * **Impact**: _Describe the effect had on the attacknet [1 to 2 sentences]_

    * **Details**: _Very specific details about the attack including the specific slots/epochs where it can be observed_

## Privacy

The Ethereum Foundation is not responsible for any private information that might
be leaked as a result of this program.

In the event that the reporting of an attack _does leak_ private information
(e.g. logs from a testnet containing IP addresses), we ask that you withhold any such information in the public report.
Instead, please note that there are additional accompanying resources to be shared,
and the attacknet evaluators will be in touch.

## Important legal information

This attacknet program is an experimental and discretionary rewards program for
our active Ethereum community to encourage and reward those who are helping
to improve the platform. It is not a competition. You should know that we can
cancel the program at any time, and rewards are at the sole discretion of Ethereum Foundation.
In addition, we are not able to issue rewards to individuals who are on sanctions
lists or who are in countries on sanctions lists (e.g. North Korea, Iran, etc).
You are responsible for all taxes. All rewards are subject to applicable law.
Finally, your testing must not violate any law or compromise any data that is not yours.


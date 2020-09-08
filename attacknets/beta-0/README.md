# [DEPRECATED] Single-client `beta-0` attacknets

_`beta-0` attacknets are deprecated. All nodes are have been disabled
and attacks/rewards are no longer eligible._

Active `beta-0` attacknets:
* [`lighthouse-attack-0`](./lighthouse-attack-0)
* [`prysm-attack-0`](./prysm-attack-0)
* [`teku-attack-0`](./teku-attack-0)

`lighthouse-attack-0`, `prysm-attack-0`, and `teku-attack0` are real networks, ready for you to attack.
These networks are single client and very small (only 4 nodes each!) so if you
have even a moderate exploit, they should be pretty easy to take down.

See each network README for specific configuration details on the network.

## Rules

Please see [general attacknet rules](../../README.md#general-rules) in addition
to the following:

* **The goal**: _Prevent finality on a single network for 16 continuous epochs_
* **The rules**:
    * Additional validators for attack are _not_ allowed and are prevented
      through a modified deposit contract.
    * "Trivial DoS attacks" are now out of scope. More novel DoS attacks that are heightened due
      to message-type/contents, packet structure, etc are still valid.
    * All other attack vectors are in scope.
    * _Show your work_. To qualify for the reward, you must (1) point specifically to the epoch range that affected,
      (2) provide some sort of proof that you caused the outage,
      and (3) provide technical details about the attack and how it was performed.
* **The reward**: _**$5k (USD)** to those that achieve the goal._ In the event
  that a network is unstable due to a prior attack, please wait until the
  network is stablized or completed restarted so we can cleanly assess and
  understand the different attack vectors.

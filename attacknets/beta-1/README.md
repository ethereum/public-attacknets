# Multi-client `beta-1` attacknets

Active `beta-1` attacknets:
* [`mc-attack-0`](./mc-attack-0)

`mc-attack-0` is a step up from the `beta-0` attacknets. `mc-attack-0` is
composed of 15 validating nodes split across three clients and has tiered
bounties up to $15k.

See the network README for specific configuration details.

## Attacker validators

In `beta-1` attacknets, potential attackers can add additional validators under
their control upon request. The attacknets use a modified deposit contract with
access control features.

Attacker validators will be alloted only up until attacknet maintainers
control a minimum of 75% of the validators. Beyond this number, attacknet
maintainers will either add more validators under their direct control or
create an additional network.

Please use this [issue template](https://github.com/ethereum/public-attacknets/issues/new?assignees=djrtwo&labels=&template=request-attacknet-validators.md&title=%5BRequest%5D+Attacknet+Validators)
to request validators.

## Rules

Please see [general attacknet rules](../../README.md#general-rules) in addition
to the following:

* **The rules**:
    * Attacker validator deposits are allowed but restricted with access control.
      See [attacker validators](#attacker-validators) for details on making a
      formal request.
    * "Trivial DoS attacks" are now out of scope. More novel DoS attacks that are heightened due
      to message-type/contents, packet structure, etc are still valid.
    * All other attack vectors are in scope.
    * _Show your work_. To qualify for the reward, you must (1) point specifically to the epoch range that affected,
      (2) provide some sort of proof that you caused the outage,
      and (3) provide technical details about the attack and how it was performed.
* **Goals and rewards**:
    * Single-client DoS vectors are not in scope.
      Use [beta-0](../beta-0) attacks to test non-trivial, client-specific DoS vectors.
    * $15k (USD) reward tier
        * sustained network split of all nodes of 1 client from others (> 16 epochs)
        * consensus split of 1 client type from others
        * multi-client DoS vector able to disrupt finality (> 16 epochs) or
          take a set of nodes entirely offline
    * $7.5k (USD) reward tier
        * sustained split of 1 node from others (> 16 epochs)
        * multi-client DoS vector able to induce a higher than normal (> 1.5x)
          resource consumption
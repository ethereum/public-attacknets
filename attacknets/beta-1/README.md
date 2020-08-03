# Multi-client `beta-1` attacknets

Active `beta-1` attacknets:
* [`mc-attack-0`](./mc-attack-0)

`mc-attack-0` is a step up from the `beta-0` attacknets. `mc-attack-0` is
composed of 15 validating nodes split across three clients and has tiered
bounties up to $15k.

See the network [README](./mc-attack-0) for specific configuration details.

## Attacker validators

In `beta-1` attacknets, potential attackers can add additional validators under
their control upon request. The attacknets use a modified deposit contract with
access control features.

Attacker validators will be alloted only up until attacknet maintainers
control a minimum of 75% of the validators. Beyond this number, attacknet
maintainers will either add more validators under their direct control or
create an additional network to maintain baseline network stability.

Please use this [issue template](https://github.com/ethereum/public-attacknets/issues/new?assignees=djrtwo&labels=&template=request-attacknet-validators.md&title=%5BRequest%5D+Attacknet+Validators)
to request validators.

## DoS Attacks

DoS vectors that are particular to a single client implementation are _not_ in
scope for `beta-1` attacknets. Please see [`beta-0`](../beta-0) attacknets for
this type of bounty.

Only "multi-client" DoS vectors are in scope in `beta-1`. That is, DoS vectors
that emerge due to having multiple implementations on the network. An example of a
multi-client DoS vector is a "reflection DoS" attack in which the insertion
of a message into the p2p network is amplified via the participating nodes
themselves.

## Rules

Please see [general attacknet rules](../../README.md#general-rules) in addition
to the following:

* **The rules**:
    * Attacker validator deposits are allowed but restricted with access control.
      See [attacker validators](#attacker-validators) for details on making a
      formal request.
    * Single-client DoS vectors are not in scope.
      Use [beta-0](../beta-0) attacks to test non-trivial, client-specific DoS vectors.
    * "Trivial DoS attacks" are not in scope. More novel DoS attacks that are heightened due
      to message-type/contents, packet structure, etc are still valid.
      See [above](#dos-attacks) for more information on DoS attacks in `beta-1`.
    * All other attack vectors are in scope.
    * _Show your work_. To qualify for the reward, you must (1) point specifically to the epoch range that affected,
      (2) provide some sort of proof that you caused the outage,
      and (3) provide technical details about the attack and how it was performed.
* **Goals and rewards**:
    * $15k (USD) reward tier
        * sustained network split of all nodes of 1 client from others (> 16 epochs)
        * consensus split of 1 client type from others
        * multi-client DoS vector able to disrupt finality (> 8 epochs) or
          take a set of nodes entirely offline
    * $7.5k (USD) reward tier
        * multi-client DoS vector able to reduce the majority of nodes' peer
          count to less than 5
    * $1 to $15k (USD) reward tier
        * novel and interesting attacks not explicitly mentioned above (rewards
          made at the discretion of attacknet maintainers)
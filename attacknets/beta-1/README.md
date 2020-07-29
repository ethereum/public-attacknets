# Multi-client `beta-1` attacknets

Active `beta-1` attacknets:
* [`mc-attack-0`](./mc-attack-0)

`mc-attack-0` is a step up from the `beta-0` attacknets. `mc-attack-0` is
composed of 15 validating nodes split across three clients and has tiered
bounties up to $15k.

See the network README for specific configuration details.

## Rules

Please see [general attacknet rules](../../README.md#general-rules) in addition
to the following:

* **The rules**:
    * "Trivial DoS attacks" are now out of scope. More novel DoS attacks that are heightened due
    to message-type/contents, packet structure, etc are still valid.
    * All other attack vectors are in scope.
    * _Show your work_. To qualify for the reward, you must (1) point specifically to the epoch range that affected,
      (2) provide some sort of proof that you caused the outage,
      and (3) provide technical details about the attack and how it was performed.
* **Goals and rewards**:
    * DoS vectors are not in scope.
      Use [beta-0](../beta-0) attacks to test non-trivial, client-specific dos vectors.
    * $15k reward tier
        * sustained network split of all nodes of 1 client from others (> 16 epochs)
        * consensus split of 1 client from others
    * $7.5k reward tier
        * sustained split of 1 node from others (> 16 epochs)
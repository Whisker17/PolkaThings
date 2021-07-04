# Security of the network

## Shared security

shared security means that all parachains that are connected to the Polkadot Relay Chain by leasing a parachain slot will benefit from the economic security provided by the Relay Chain validators.

The notion of shared security is different from interchain protocols that build on an architecture of bridges. For bridge protocols, each chain is considered sovereign and must maintain its own validator set and economic security. One concern in these protocols is on the point of scalability of security.

Polkadot overcomes security scalability concerns since it gravitates all the economic incentives to the **Relay Chain** and allows the parachains to tap into stronger guarantees at genesis. Sovereign chains must expend much more effort to grow the value of their coin so that it is not easily attackable by well-funded attackers.



**Security is independent of the number of parachains that are connected to the Polkadot Relay Chain.** 

The correlation of security and the number of validators exists as the higher number of validators will give the network stronger decentralization properties and make it harder to try to take down. However, the biggest indicator of the security of the network is the economic signal of the number of DOT that are bonded and staked. The greater the number of DOT staked by honest validators and nominators, the higher the minimum amount of DOT an attacker would need to acquire a validator slot.



Most parachains will not need to worry about their own security, since all state transitions will be secured by the Polkadot Relay Chain validator set. However, in some cases (which are considered more experimental), parachains may require their own security. In general, these cases will revolve around lack of data available to Relay Chain validators.

**ZKP**
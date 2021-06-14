# Architecture

## Relay Chain

- **Role**
  - Central chain of Polkadot.

- All validators ------(stake on and validate)----> Realy Chain
- consist of a few transaction types (governance mechanism / parachain auctions / participate in NPoS)
- not support smart contracts

## Parachain and Parathread Slots

- **Parachain -> one slot** && **Parathread -> share one slot**
- no constraints on parachains if they can proof their states
- Parachains will have to reserve DOT for duration of their slot lease; parathreads will pay on a per-block basis.
- Parachain <----> Parathread
- **Security**
  - **Parachains connected to the Polkadot Relay Chain all share in the security of the Relay Chain.**
- **Role**
  - **Validators**
    - produce blocks on the Relay Chain
    - accept proofs of valid state transition from collators
    - can get staking rewards
  - **Collators**
    - full nodes on both a parachain and the Relay Chain
    - collect parachain transactions and produce state transition proofs for Validators on the Relay Chain
    - send and receive messages from other parachains using XCMP
  - **Nominators**
    - bond stake to particular validators -> help them get into the active validator set -> produce blocks for the chain
    - get rewards from validators


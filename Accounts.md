# Polkadot Accounts

## Address

### Address Format

- Substrate-based chains -> [**SS58**](https://github.com/paritytech/substrate/wiki/External-Address-Format-(SS58)) (A modification of Base58 from Bitcoin)
  - **Polkadot addresses start with 1**
  - **Kusama addresses start with a capital letter**
  - **Generic Substrate addressese start with 5**

- Same private-public keypair -> different representations of the same public key
- [Address transform tools](https://polkadot.subscan.io/tools/ss58_transform) 

### Address Generation, Derivation, and Portability

- supported curves and signature schemes
  - Ed25519
  - Sr25519 - Schnorr signatures on the Ristretto group
  - ECDSA signatures on secp256k1
- Seed
  - [Substrate BIP39](https://github.com/paritytech/substrate-bip39) 

- Subkey is a public key cryptographic utility that is developed within Substrate itself
  - [Installation](https://substrate.dev/docs/en/knowledgebase/integrate/subkey)

- **Portability**
  - Portability depends on a number of factors:
    - Derivation path
    - Mnemonic format
    - Seed derivation
    - Signature scheme

- Prefix
  - Polkadot has an address type of `00000000b`, so `0` in decimal.
  - Kusama (Polkadot Canary) has an address type of `00000010b`, so `2` in decimal.
  - Generic Substrate has `00101010b` as address type, which is `42` in decimal.

- Balance Types
  - free
  - reserved
  - misc_frozen / miscFrozen
  - fee_frozen / feeFrozen

- Multi-signature Accounts
  - A multi-signature account is composed of one or more addresses and a threshold.
  - Multi-signature accounts **cannot be modified after being created**.
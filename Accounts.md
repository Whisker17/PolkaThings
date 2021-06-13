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

- 
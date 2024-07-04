# cardano-purescript [![cardano-purescript](https://img.shields.io/badge/cardano--purescript?logo=cardano&logoColor=white&label=cardano-purescript&labelColor=blue&color=blue)](https://github.com/klntsky/cardano-purescript)

This is an overview of open source PureScript (and JavaScript) packages that facilitate Cardano dApp development.

## PureScript packages

- [cardano-transaction-lib](https://github.com/Plutonomicon/cardano-transaction-lib) -  A Purescript framework for building smart contract transactions on Cardano
- [purescript-cardano-types](https://github.com/mlabs-haskell/purescript-cardano-types) - domain types for Cardano ledger, wraps `purescript-cardano-serialization-lib`.
- [purescript-cardano-serialization-lib](https://github.com/mlabs-haskell/purescript-cardano-serialization-lib) - PureScript wrapper for CSL.
- [purescript-plutus-types](https://github.com/mlabs-haskell/purescript-plutus-types) - Plutus-style types used for their PlutusData instances.
- [purescript-cardano-plutus-data-schema](https://github.com/mlabs-haskell/purescript-cardano-plutus-data-schema) - machinery for specifying PlutusDataSchema (PlutusData encoding layouts for PureScript algebraic data types) in CTL
- [purescript-cardano-collateral-select](https://github.com/mlabs-haskell/purescript-cardano-collateral-select/) - collateral selection algorithm that tries to minimize min-ADA value
- [purescript-uplc-apply-args](https://github.com/mlabs-haskell/purescript-uplc-apply-args) - apply `PlutusData`-encoded parameters to parametrized Plutus scripts
- [purescript-cip30-typesafe](https://github.com/mlabs-haskell/purescript-cip30-typesafe) - safe error handling for CIP-30 wrappers
  - [purescript-cip30](https://github.com/mlabs-haskell/purescript-cip30) - CIP-30 API wrappers (no error handling)
- [purescript-cardano-message-signing](https://github.com/mlabs-haskell/purescript-cardano-message-signing) - implementation of CIP-8/CIP-30 `signData`, purescript wrapper over [`Emurgo/message-signing`](https://github.com/emurgo/message-signing)
- [purescript-cardano-hd-wallet](https://github.com/mlabs-haskell/purescript-cardano-hd-wallet) - implementation of [CIP-1852](https://cips.cardano.org/cip/CIP-1852) using `cardano-serialization-lib` (private key derivation from mnemonics)
- [purescript-noble-secp256k1](https://github.com/mlabs-haskell/purescript-noble-secp256k1/) - cryptographic functions needed to work with Vasil hardfork features
- [purescript-aeson](https://github.com/mlabs-haskell/purescript-aeson/) - partial re-implementation of Argonaut with support of unquoted long integers - can be used for interoperability with Aeson, that encodes long integers unquoted. We need this for interactions with Cardano tooling in Haskell
  - [json-bigint](https://github.com/mlabs-haskell/json-bigint) - big integer machinery (JavaScript)
- [purescript-bytearrays](https://github.com/mlabs-haskell/purescript-bytearrays) - byte string type and utilities
- [purescript-mote-testplan](https://github.com/mlabs-haskell/purescript-mote-testplan) - effectful testplans for [Mote](https://github.com/garyb/purescript-mote), a testing library

## JavaScript packages

- [@mlabs-haskell/cardano-serialization-lib-gc](https://github.com/mlabs-haskell/cardano-serialization-lib-gc) - CSL version vendored by MLabs, with automatic GC added
  - [@mlabs-haskell/csl-gc-wrapper](https://github.com/mlabs-haskell/csl-gc-wrapper) - Garbage collector for CSL
- [@mlabs-haskell/uplc-apply-args](https://github.com/mlabs-haskell/uplc-apply-args) - JavaScript package for Plutus script parameter application

## Work in progress

These packages haven't been fully finalized:

- [purescript-cardano-transaction-builder](https://github.com/mlabs-haskell/purescript-cardano-transaction-builder) - Declarative transaction builder API & utility functions for automatic redeemer indexing
- [purus](https://github.com/mlabs-haskell/purus) - A fork of the PureScript compiler that compiles to Untyped Plutus Core - smart contract language of Cardano

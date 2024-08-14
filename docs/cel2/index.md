---
title: Introduction to Celo Layer 2
description: Introducion to Cel2
---

Celo is transitioning from a standalone EVM-compatible Layer 1 blockchain to an Ethereum Layer 2. 
This shift, proposed by cLabs in July 2023, aims to maintain the seamless user experience that
Celo is known for—characterized by speed, low costs, and ease of use—while leveraging Ethereum’s 
security and ecosystem. As part of this transition, Celo is currently operating two Layer 2 testnets:
Dango, which is live, and Alfajores, which will be upgraded to Layer 2 in late September 2024.


## Alfajores L2 Upgrade

The Alfajores testnet is set to upgrade to Layer 2 in late September 2024. This upgrade will transition 
Alfajores into the Celo Layer 2 environment, allowing developers and integrators to start building and 
testing with the new infrastructure. This is a key step in Celo’s broader evolution, paving the way for 
future upgrades to the Baklava testnet and the mainnet.

## Dango Testnet

The Dango Testnet, Celo’s first Layer 2 public test network, is currently live. Dango allows developers
and infrastructure providers to familiarize themselves with the Layer 2 environment. 
Key features of Dango include:

- Full Alfajores history and state
- CELO token duality (ability to use CELO natively and as an ERC20 token)
- Fee abstraction (ability to pay for gas with tokens)
- Native Bridging to and from the L1
- Data Availability via EigenDA
- Staking
- Ultragreen Money

:::warning
The Dango Testnet is designed preliminary for testing and experimentation by developers. Its tokens hold no real world economic value. You may encounter bugs and limitations with the software and documentation.
:::

## Getting Started with Dango

Information and resources to get you started:

- RPC URL: https://forno.dango.celo-testnet.org/
- Explorer: https://celo-dango.blockscout.com/
- ChainID: 44787

:::warning
Please note that the Dango chain ID remains the same as Alfajores, ensuring seamless functionality but introducing the possibility of replay attacks where transactions could be replayed between Dango and Alfajores.
:::

## CeloCLI

1. Setup celo-cli

```bash
celocli config:set --node https://forno.dango.celo-testnet.org/
```

2. Check balance of a Cel2 account

```bash
celocli account:balance $ACCOUNT_ADDRESS --node https://forno.dango.celo-testnet.org/
```

## Useful Links

- [Add Cel2 Dango Testnet to Metamask](/docs/cel2/add-cel2-testnet-to-metamask.md)
- [Dango Faucet](https://faucet.celo.org/dango)
- [Dango Block Explorer by Blockscout](https://celo-dango.blockscout.com/)
- [Superchain Bridge for migrating assets from L1 to L2](https://testnets.superbridge.app/)
- [Layer 2 Specification](https://specs.celo.org/root.html)
- [FAQ](https://docs.celo.org/cel2/faq)
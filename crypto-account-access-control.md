---
title: 🫱🏻‍🫲🏼 Crypto account access control
tags: Crypto
description: Access control for crypto accounts
---

<h1 style="text-align: center;">🫱🏻‍🫲🏼 Crypto account access control</h1>

# Sign-in use case

#### About

- Accounts should follow the [principle of least privilege (PoLP)](https://en.wikipedia.org/wiki/Principle_of_least_privilege) to expose the least amount of data necessary.
- Tokens like NFTs are used for gated communities, products, and services.
- Storing valuable tokens on less secure hot wallets is risky.
- Storing valuable tokens on more secure cold wallets and multisig wallets is not easy to use.
- Aka account/wallet/token/app permissions/delegation

#### Assign access controls for sign-in

- Assign flexible and custom access to apps
    - E.g. Allow a hot wallet to claim airdrops that are deposited into cold storage
- [@DCInvestor 2022-12-20](https://twitter.com/iamDCinvestor/status/1605200387694280704?t=3SL6OK9-kRjkpz6_QuZY3A&s=09)
- Alternative: Web and app based credential storage with cookies

# Delegate Cash

*[delegate.cash](https://delegate.cash/)*

#### About

- Provide access and features from secure wallets to easily accessible wallets that is open and immutable.
- Secures $228mm+ in assets (2023-01-19): [@beetle / Total Delegated Value](https://dune.com/queries/1649062/2733111) *on Dune Analytics*
- Twitter: [@delegatecash](https://twitter.com/delegatecash)
- [delegate.cash](https://0xfoobar.substack.com/p/delegatecash) *by foobar 2022-09-28*

#### Delegation features

- Tokens like ERC-20, NFTs like ERC-721, and etc.
- Contracts like Uniswap and LensProtocol
- Wallet addresses

#### Networks
- Ethereum, Polygon, and Goerli (Compatible on all EVM protocols)

#### Implementation options

A. Smart contract
B. Javascript SDK/API
C. Integrate with a trusted provider who has integrated, e.g. A bridging service.

#### Steps to use

1. From a secure wallet assign a hot wallet delegate.
    a. Assign for all assets
    b. Assign for a specific contract
    c. Assign for a specific token
2. The delegate has permission to use the assigned tokens, e.g, Sign-in, claim airdrops, and etc.
    a. The delegate cannot move or access any other tokens or assets in the original secured wallet.

#### Architecture

- Uses singleton pattern.
- Integrations query the central registry rather than deploy their own.
- Requires that the smart contract interacting with the user wallet recognizes the Delegate.cash registry as a source of truth.

#### Opportunities

- Public audits on the Delegate.cash contract
- [EIP-5639: Delegation Registry](https://eips.ethereum.org/EIPS/eip-5639) adoption
- [Safe](https://hackmd.io/@safe/og/https%3A%2F%2Fhackmd.io%2F%40safe%2Fopportunities#Access-control-P1) support

#### Open-source

- Contract: [0x00000000000076A84feF008CDAbe6409d2FE638B](https://etherscan.io/address/0x00000000000076a84fef008cdabe6409d2fe638b)
- UI: [github.com/0xfoobar/delegate-cash-frontend](https://github.com/0xfoobar/delegate-cash-frontend)
- Registry: [github.com/delegatecash/delegation-registry](https://github.com/delegatecash/delegation-registry)

# Delegatable

*[delegatable.org](https://delegatable.org)*

#### About

- Created by [Dan Finlay](https://twitter.com/danfinlay), MetaMask Co-founder
- Contract based
    - Access control features built into the contract rather than a contract needing to be updated in order to accept an outside registry.
    - Uses off-chain signatures
- Open-source

#### Related topics

- [Better Dapps with Delegatable ](https://www.youtube.com/watch?v=NMqaCGxSRQY) *by Dan Finlay at ETHDenver on YouTube 2023-03-02*
    - [Delegatable compared to Delegate.cash and warm (24:06)](https://youtu.be/NMqaCGxSRQY?t=1446)
        - Delegatable: Smart contract based? *by [@adamshurwitz Tweet 2023-03-02](https://twitter.com/adamshurwitz/status/1631500487701962752)*
        - Delegate.cash and Warm: Registry based

# Sismo

*[Sismo.io](https://sismo.io)*

#### About

- Maintains the privacy of connected accounts
    - Compared to other contract and registry delegation strategies that potentially expose the account addresses.
- Open-source
- Compatible for EVM protocols
- Twitter: [@Sismo_eth](https://twitter.com/Sismo_eth)

#### Sign-in with Sismo (SIWS)

- 2 accounts create a Sismo vault
- Vaults store ZK badges
    - Non-transferrable NFTs, aka Soulbound tokens (ERC-1155)
    - Technically ERC-20 with badge balances
    - Minted by a ZK attester smart contract
- Connect to the third-party service with the vault
- Transferring badges
    - Can create new badges with the attester contract

#### Related topics

- [StarkWare Sessions #5 | Starknet Identity with Hadrien of Sismo](https://pca.st/vddaub70) *by Bankless 2023-02-11*
- [ZK Badges: A new primitive for self sovereign identities by dhadrien | Devcon Bogotá](https://www.youtube.com/watch?v=6vCb6XwGSOk) *on YouTube 2022-10-15*

#### Research

- Is the ZK attester contract immutable by anyone? *by [@adamshurwitz Tweet 2023-03-02](https://twitter.com/adamshurwitz/status/1631513005874900992)*

# Warm

*[warm.xyz](https://warm.xyz)*

#### About

- Registry-based (Similar to Delegate.cash)
- You can only delegate access to your cold wallet to a single hot wallet at a time: [warm.xyz/faq](https://warm.xyz/faq) > *How do I use Warm?*

# Research to dos

## Return on investment (ROI)

- Metric: How much USD value is secured with each access control solution?
- Opportunity size    
    - Project based on YoY user metrics (transaction volume, sign-ins, and etc.) of sign-in with Ethereum (SIWE) apps.
        - Individuals
            - Financial
            - Social: Lens apps, Farcaster, Skiff, etc
            - Top NFT projects
            - Top games
        - Organizations
    - Total USD value of high-profile hacks in crypto.

## Decentralization

- Which solutions are the most trustless? That is do they require trust in a third party for the off-chain transactions?

<p style="text-align: center; font-style: italic">This content is not financial or technical advice. Always consult a financial professional and do your own research.
</p>
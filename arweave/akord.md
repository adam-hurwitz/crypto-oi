---
title: 🅰 Akord
tags: crypto
description: Akord decentralizatd and encrypted file storage.
image: https://pbs.twimg.com/profile_banners/3540691454/1535710532/1500x500
---

<h1 style="text-align: center;">🅰 Akord</h1>

<p style="text-align: center; 
          font-style: italic;">
    <a href="https://akord.com" target="_blank">akord.com</a>
</p>

# About

#### Overview

- Permanent data storage
    - Including photos, video, and audio player
    - Publishing with Markdown language
    - Pay with Stripe in local currency
- [Permaweb Publishing](https://akord.com/products/web-app)
- [API & Builder Tools](https://akord.com/products/api)
- Future collective profit-sharing model with $AKRD
    - [$AKRD token](https://docs.akord.com/overview/about/usdakrd-token)
    - [Time to drop Dropbox](https://akord.com/blog/time-to-drop-dropbox) *2022-05-22*
- Documentation: [docs.akord.com](https://docs.akord.com)
    - Potentially to host docs on Arweave: [@AkordTeam 2022-01-19](https://twitter.com/AkordTeam/status/1616076783757193218)

#### Community and support

- Twitter: [@AkordTeam](https://twitter.com/AkordTeam)
- Discord: [discord.com/invite/YQVAyhFgAn](https://discord.com/invite/YQVAyhFgAn)
- Show: [Striking Akord](https://pca.st/ovg8l9ep)
- Blog: [akord.com/blog](https://akord.com/blog)
- Support: [support@akord.com](mailto:support@akord.com)

# Features

#### Vaults

- Encrypted
    - End-to-end encrypted (E2EE)
    - Private encrypted and share options
    - Encrypted files are available for anyone to download
    - Current AES-256 encryption requires $2.29x10^{32}$ years

- Public
    - Not end-to-end encrypted (E2EE)
- Terms of access (ToA)
    - You can add terms of access to be digitally signed before someone is added to a vault.
- Creating vaults and uploading files takes time depending on the data transactions settling on the Arweave network.
    - Based on the Arweave network demand and bandwidth.
    - *See [How long do transactions take to confirm?](https://docs.akord.com/v/app-docs/frequently-asked-questions/how-long-do-transactions-take-to-confirm)*
- Revoke files
    - Cannot delete files because data stored on Arweave is permanent
    - Revoking prevents anyone from renaming, moving, downloading, or viewing the file.
        - The file continues to exist.
        - The file remains encrypted and is therefore useless. 
    - Opportunity
        - Remove revoked files from the Arweave network: [@adamshurwitz Tweet 2023-04-30](https://twitter.com/adamshurwitz/status/1652718211052322817)
    - Resources
        - Arweave content moderation: [Open info](https://hackmd.io/@openinfo/arweave#Content-moderation)
        - [Can I delete files from permanent storage?](https://docs.akord.com/v/app-docs/frequently-asked-questions/can-i-delete-files-from-the-blockchain)

#### Messaging

- End-to-end encrypted (E2EE) messaging between Akord accounts

#### Security

- End-to-end-encryption (E2EE) with zero-knowledge proofs (ZKPs)
    - [End-to-end encryption](https://docs.akord.com/learn/end-to-end-encryption)
- Multi-factor authentication (MFA)
    - App
    - SMS
- Permanent data storage
    - [Arweave protocol](https://docs.akord.com/v/app-docs/arweave/arweave-protocol)
- Decentralization with Akord Explorer
    - [What if Akord no longer exists?](https://docs.akord.com/v/app-docs/frequently-asked-questions/what-if-akord-no-longer-exists)
- *See [Akord protocol – open for builders](https://akord.com/blog/the-akord-protocol-open-for-builders) 2022-09-26*

#### Open-source

- [github.com/Akord-com](https://github.com/Akord-com)
- AkordJS: Interacting with vaults
    - [AkordJS: privacy, collaboration and file management on Arweave](https://akord.com/blog/akordjs-privacy-collaboration-and-file-management-on-arweave) *2023-01-30*

# Opportunities

## Open

#### Download directories containing child directories (P0)

- The downloaded directory only contained it's "1st level of child files" and no "2nd level of directories".
- E.g. Download a `build-oi` folder.
  - Downloaded successfully
    - `build-oi/artificial-intelligence-ai.md`
    - `build-oi/markdown.md`
    - `build-oi/open-information-oi.md`
    - `build-oi/skiff.md`
  - Did not download
    - `build-oi/.git/...`
    - `build-oi/hackmd/...`
- *See [Discord post 2023-06-27](https://discord.com/channels/890229689019432981/890867529231237140/1123344661545758720)*

#### Show potential causes for files not uploading. (P1)

- [Screenshot 2023-03-13](https://drive.proton.me/urls/KQV6V4YCHM#cL8rBHUDdpMF)

#### Upload multiple folders at once. (P1)

#### Desktop syncing app (P1)

- Similar to Dropbox and Google Drive's apps

#### Mobile apps (P2)

#### Keyboard shortcuts for basic actions (P2)

## Fixed

#### Files show at the vault root level when they are uploaded instead of the current directory location (P0)

- Fixed 2023-06-20

<p style="text-align: center; font-style: italic">This information is not financial or technical advice. Always consult a financial professional and do your own research.</p>
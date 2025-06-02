Title: Enable Multi-Wallet Import and Aggregation Across Infinex Accounts
Author: Dr.Acay
Type: XIP (Core Upgrade)
Status: Draft
Created: 2025-06-02
Network: Infinex (Multi-chain)

Proposal Summary
This XIP proposes the ability for users to import and manage multiple external wallets within a single Infinex account. This feature would enhance the platform's functionality by providing a unified portfolio view and allowing for consolidated governance participation, trading, and staking across all connected wallets.

Specification
Key Features:
Multi-Wallet Import
Users can import EVM-compatible wallets (e.g., MetaMask, WalletConnect, hardware wallets) and view them alongside their Infinex-native wallet.

Read-Only or Active Permissions
Users can choose to import wallets in:

Read-only mode (for viewing balances and transaction history)

Active mode (to allow trades, voting, or transfers via signatures)

Unified Portfolio Dashboard
Aggregates assets from imported wallets across all supported chains (Solana, Ethereum, Arbitrum, Optimism, Base, Blast, etc.) into a single dashboard view.

Governance Integration
Imported wallets that hold eligible assets (e.g., Patron NFTs, staked SNX) can contribute to governance voting and proposal submissions via signature verification.

Security & Privacy
Imported wallets remain non-custodial. Private keys are not stored by Infinex. Wallet actions require explicit user authorization via signature for every interaction.

Revocation and Management
Users can revoke any imported wallet at any time. Wallets can be renamed for personal convenience.

Rationale
Most DeFi users interact with multiple wallets across different chains. Enabling wallet imports enhances the user experience by removing the need to switch between wallets, simplifies tracking of funds, and reduces governance fragmentation. It also aligns Infinex with wallet aggregation standards seen in apps like Zapper and DeBank, but with deeper governance and trading integration.

Technical Specification
Feature	                                Specification
Import Types	                  WalletConnect, Private Key, Ledger/Trezor
Supported Chains	              Solana, Ethereum, Base, Arbitrum, Optimism, Blast
Access Modes	                  Read-Only, Active (signed actions only)
Integration	                    Trading, Governance, Leaderboards
Security Model	                Non-custodial, signature-based access only

Security Considerations
.No private key storage.
.Every transaction requires user confirmation.
.Read-only wallets cannot initiate actions.
.Metadata (wallet nicknames, tags) stored locally or encrypted server-side.

Copyright
CC0 – No rights reserved.

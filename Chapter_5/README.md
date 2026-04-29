## Concordium: Sponsored Transactions
This workshop provides an introduction to Concordium's Sponsored Transactions feature, a key component for enabling mass adoption by simplifying the user experience. The session explains how this feature removes the friction of needing native gas tokens for transactions.

## The Concordium Stack
The Chapter began with a quick review of core Concordium concepts covered in previous Chapter:

## Protocol-Level Identity:
Every account is tied to a verified identity, ensuring compliance without storing personal data on-chain.
Verify & Access: A system using Zero-Knowledge (ZK) proofs to verify user attributes (like age or nationality) without revealing the underlying data.
Protocol Level Tokens (PLTs): Natively managed tokens (CIS-7 standard) that are not dependent on smart contracts, offering enhanced security and self-custody.
The Core Problem: Dual-Token Friction
A major barrier to entry in many blockchain applications is the dual-token problem. This occurs when a user wants to transact with a specific token (e.g., a stablecoin) but is required to also hold the blockchain's native token (e.g., CCD) just to pay for the transaction fee. This is confusing for new users and creates a poor, multi-step user experience.

## Key Takeaway:
Sponsored Transactions solve this by allowing a third party (a "sponsor," typically the dApp or merchant) to pay the CCD transaction fee on behalf of the user. The user only needs to hold and approve the token they actually want to spend.

How Sponsored Transactions Work
Introduced in Protocol 10, this feature is built directly into the blockchain, not as a smart contract workaround.

## Signing Flow:
The process requires two signatures: 1) The sender signs the transaction payload (e.g., authorizing the transfer of 50 EURR), and 2) The sponsor signs to cover the CCD fee.
Sequence Numbers (Nonce): To prevent replay attacks, only the sender's sequence number is consumed. This is crucial because it means a sponsor can process thousands of transactions for different users without creating sequencing conflicts for their own account's operations.
Cost-Effective: The fee is a predictable ~€0.01 per transaction, making it scalable for businesses to sponsor transactions at a large scale.
Live Demo & Architecture
The workshop included a live demo showing a user with zero CCD successfully sending a PLT (stablecoin) transaction. The dApp's backend service acted as the sponsor, building the transaction, signing its portion, and then passing it to the user's wallet for final approval. The user experience was seamless, with the wallet simply showing a "Free Transaction."

## Use Cases
The potential applications are broad, enhancing any user-facing dApp:

Age-gated E-commerce: A customer can prove they are over 18 with a ZK proof and pay with a stablecoin, while the merchant sponsors the fee. The entire process is settled in ~4 seconds with no GDPR liability for the merchant.
Cross-border B2B Settlements: Drastically reduces the time (from 1-5 days to ~4 seconds) and cost of international payments compared to traditional SWIFT wires.
Online Gaming: Platforms can sponsor all fees, allowing players to interact with stablecoins without needing to understand gas fees, creating a frictionless experience.

# Introduction to Concordium: Identity On-Chain Educate Series
This session kicks off a seven-week educational series focused on Concordium's unique approach to on-chain identity. Hosted by Encode Club, the program is designed to give developers a deep understanding of how to build with Concordium's privacy-preserving, regulatory-compliant blockchain. 

## Why Concordium Exists: Solving Blockchain's Identity Problem
Dragos Danciulescu from Concordium explained the core challenges of current public blockchains:

Anonymity vs. Pseudonymity: Most chains are either fully anonymous (hindering regulation) or pseudonymous (lacking privacy), creating friction for enterprise and financial applications.
Market Need: The market requires a solution that offers accountability while maintaining privacy, auditability, and protocol-level compliance.
Core Design Principles of Concordium
Concordium is a public, permissionless blockchain designed to bridge this gap with several key principles:

Privacy by Default: User transactions are private, with accountability enforced by law only when necessary.
Fast Finality: Transactions are finalized in approximately 4 seconds.
Predictable Fees: Transaction fees are pegged to the Euro for stability.
Regulatory-Ready Infrastructure: Built from the ground up to support compliance.
Rust-Based Smart Contracts: Utilizes the secure and performant Rust programming language.
Technical Architecture & Tooling
The presentation detailed Concordium's layered architecture, featuring a distinct Identity Layer paired with the Execution Layer. This unique structure works with external identity providers to verify real-world identities off-chain while preserving user privacy on-chain through zero-knowledge proofs.

## Getting Started: Local Chain Demo
A significant portion of the session was a practical demonstration on setting up a local Concordium blockchain environment using a pre-packaged Docker compose setup. This sandbox allows developers to spin up a complete local network, including:

A Concordium protocol node with gRPC.
A test identity provider.
Wallet Proxy and CCDscan Blockchain Explorer.
A full database and web server setup.
This local environment enables developers to test smart contracts, create protocol-level tokens (PLTs), and interact with the entire ecosystem without needing to connect to a public testnet or mainnet.

## Concordium: Protocol Level Tokens (PLTs)
This Chapter explores Concordium's innovative approach to digital assets, moving beyond traditional smart contract tokens to a more secure and efficient protocol-level implementation.

## Key Takeaway:
Concordium's Protocol Level Tokens (PLTs) are designed as "smart money, not just smart contracts," offering built-in security, compliance, and predictable costs by integrating token logic directly into the blockchain protocol layer.

## Part 1:
The Problem with Smart Contract Tokens & The PLT Solution
The session begins by outlining the inherent risks and inefficiencies of smart contract-based tokens like ERC-20:

## Security Vulnerabilities:
Every custom smart contract introduces a new attack surface, leading to risks like re-entrancy hacks, honeypots, and hidden functions. Billions have been lost to such exploits.
## High & Unpredictable Costs:
Gas fees for smart contract execution can be variable and expensive.
## No Built-in Compliance:
Compliance features like KYC and allowlists must be bolted on after the fact, leading to inconsistency and fragmentation.
Concordium's answer is Protocol Level Tokens (PLTs), which are issued and managed natively at the protocol level. This design provides:

## Enhanced Security:
A much smaller, standardized, and vetted attack surface.
## Predictable Costs:
Fixed, low transaction fees (approx. €0.01).
## Built-in Compliance & Governance: Core logic for minting, burning, transfers, and access control (allowlist/denylist) is part of the protocol itself.
## Part 2:
Technical Deep Dive & dApp Demo
This section details the practical implementation and unique features of PLTs.

## Self-Custody by Design:
Unlike many smart contract tokens held in the contract's state, PLTs are always held directly in the user's wallet, ensuring the user maintains control of their keys.
## Verify & Pay:
A powerful feature combining Concordium's Identity Layer with its payment layer. A user can prove an identity attribute (e.g., age > 18) via a ZK proof and execute a PLT payment in a single, seamless flow, without revealing their identity.
## Allowlist Manager Faucet dApp Demo: A practical demonstration showed a dApp where users:
Connect their Concordium wallet.
Generate a ZK proof to verify their country of residence is within the EU.
Once verified, an atomic transaction automatically adds their account to the allowlist, mints 100 new EU-Demo tokens, and transfers them to their wallet. This showcases how multiple operations can be batched into a single, fail-safe transaction.
## Part 3:
An Issuer's Perspective with Aryze
Jody Husain, co-founder and CTO of Aryze, a regulated stablecoin issuer, shared why they chose to build on Concordium.

## Reduced Complexity & Risk:
By using PLTs, Aryze doesn't have to worry about the security and auditing of custom smart contracts. This allows them to focus on their core product.
## The Power of the Identity Layer:
The built-in identity framework is crucial for bridging the gap between the traditional financial world and the digital asset space, enabling compliant operations.
Frictionless Experience: The ability to easily issue a token with built-in governance tools provides a much simpler and more secure onboarding process for issuers.

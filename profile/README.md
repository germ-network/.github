We build end-to-end encrypted messaging in Swift, and maintain these libraries:

## Top-level protocols

The two main protocols you need to construct Germ's cross-user wire formats:

| Package | What it does | License |
| --- | --- | --- |
| [autonomous-comm-protocol](https://github.com/germ-network/autonomous-comm-protocol) | `CommProtocol` — a protocol for autonomous communication between users | MIT |
| [twomlspq-swift](https://github.com/germ-network/twomlspq-swift) | Swift-native 1:1 triple ratchet (TwoMLSPQ) | Apache-2.0 OR MIT |

## AT Protocol

A family of protocols for [atproto](https://atproto.com) clients.

| Package | What it does | License |
| --- | --- | --- |
| [AtprotoClient](https://github.com/germ-network/AtprotoClient) | AT Protocol client that takes an injected OAuth session for authenticated requests | MIT |
| [AtprotoOAuth](https://github.com/germ-network/AtprotoOAuth) | AT Protocol OAuth client | MIT |
| [AtprotoTypes](https://github.com/germ-network/AtprotoTypes) | Swift types for AT Protocol primitives, with verification and mock variants | MIT |
| [Microcosm](https://github.com/germ-network/Microcosm) | Client for the AT Protocol services on [microcosm.blue](https://microcosm.blue) | MIT |

## Spec-driven cryptography libraries

| Package | What it does | License |
| --- | --- | --- |
| [swift-mls](https://github.com/germ-network/swift-mls) | A construction kit for MLS-family protocols [(RFC 9420)](https://datatracker.ietf.org/doc/rfc9420/), built on swift-crypto | MIT |
| [swift-raae](https://github.com/germ-network/swift-raae) | Random-access authenticated encryption and the SEAL construction, per [`draft-sullivan-cfrg-raae`](https://datatracker.ietf.org/doc/draft-sullivan-cfrg-raae/03/). Pre-1.0: stored bytes are not yet stable across draft revisions | MIT |
| [TwoMLSPQ](https://github.com/germ-network/TwoMLSPQ) | A rust implementation of twomlspq. Now superceded by twomlspq-swift, but this was the original implementation that contains the protocol reference. | Apache-2.0 OR MIT |

## Other spec libraries

| Package | What it does | License |
| --- | --- | --- |
| [jxl-encoder-swift](https://github.com/germ-network/jxl-encoder-swift) | Pure-Swift lossy JPEG XL encoder (ISO/IEC 18181) — no unsafe constructs, no C dependencies; a port of libjxl-tiny verified byte-identical against it | BSD-3-Clause |
| [oauth4swift](https://github.com/germ-network/oauth4swift) | Building blocks for OAuth 2.1 clients, inspired by [oauth4webapi](https://github.com/panva/oauth4webapi) | MIT |

## Supporting libraries

| Package | What it does | License |
| --- | --- | --- |
| [GermConvenience](https://github.com/germ-network/GermConvenience) | Leaf-dependency convenience extensions shared across Germ projects (HTTP, HTTP signatures, CBOR) | MIT |
| [swift-secret-bytes](https://github.com/germ-network/swift-secret-bytes) | Zeroizing custody types for secret bytes, built around swift-crypto's `SymmetricKey` | MIT |

## In design

| Package | What it does | License |
| --- | --- | --- |
| [atproto-pmr](https://github.com/germ-network/atproto-pmr) | Interop specification for the Atproto Personal Messaging Relay — a weakly trusted, persistently online delegate of an atproto DID | MIT |

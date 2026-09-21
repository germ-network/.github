# Germ Network

We build end-to-end encrypted messaging in Swift and Rust: MLS-family and
post-quantum group protocols, the cryptographic primitives underneath them, and the
AT Protocol client tooling that carries them.

Each package's license is listed below.

## Swift packages

| Package | What it does | License | Status |
| --- | --- | --- | --- |
| [AtprotoClient](https://github.com/germ-network/AtprotoClient) | AT Protocol client that takes an injected OAuth session for authenticated requests | MIT | Active |
| [AtprotoOAuth](https://github.com/germ-network/AtprotoOAuth) | AT Protocol OAuth client | MIT | Active |
| [AtprotoTypes](https://github.com/germ-network/AtprotoTypes) | Swift types for AT Protocol primitives, with verification and mock variants | MIT | Active |
| [autonomous-comm-protocol](https://github.com/germ-network/autonomous-comm-protocol) | `CommProtocol` — a protocol for autonomous communication between users | MIT | Active |
| [DistributedMLS](https://github.com/germ-network/DistributedMLS) | Prototype Swift implementation of [draft-xue-distributed-mls](https://datatracker.ietf.org/doc/draft-xue-distributed-mls/) | MIT | Active |
| [GermConvenience](https://github.com/germ-network/GermConvenience) | Leaf-dependency convenience extensions shared across Germ projects (HTTP, HTTP signatures, CBOR) | MIT | Active |
| [jxl-encoder-swift](https://github.com/germ-network/jxl-encoder-swift) | Pure-Swift lossy JPEG XL encoder — no unsafe constructs, no C dependencies; a port of libjxl-tiny verified byte-identical against it | BSD-3-Clause | Active |
| [Microcosm](https://github.com/germ-network/Microcosm) | Client for the AT Protocol services on [microcosm.blue](https://microcosm.blue) | MIT | Active |
| [oauth4swift](https://github.com/germ-network/oauth4swift) | Building blocks for OAuth 2.1 clients, inspired by [oauth4webapi](https://github.com/panva/oauth4webapi) | MIT | Active |
| [swift-mls](https://github.com/germ-network/swift-mls) | A construction kit for MLS-family protocols (RFC 9420), built on swift-crypto | MIT | Active |
| [swift-raae](https://github.com/germ-network/swift-raae) | Random-access authenticated encryption and the SEAL construction, per `draft-sullivan-cfrg-raae`. Pre-1.0: stored bytes are not yet stable across draft revisions | MIT | Active |
| [swift-secret-bytes](https://github.com/germ-network/swift-secret-bytes) | Zeroizing custody types for secret bytes, built on swift-crypto's `SymmetricKey` | MIT | Active |
| [TwoMLSPQ](https://github.com/germ-network/TwoMLSPQ) | Post-quantum implementation of twoMLS. The Swift package is the consumable artifact — one release tag pins one (Swift API, Rust binary) pair via an xcframework URL and checksum | Apache-2.0 OR MIT | Active |
| [twomlspq-swift](https://github.com/germ-network/twomlspq-swift) | Swift-native 1:1 triple ratchet (TwoMLSPQ) | Apache-2.0 OR MIT | Active |
| [verifier-swift](https://github.com/germ-network/verifier-swift) | Tinfoil attestation verifier packaged for Swift | **None** | Active |
| [ATProtoLiteClient](https://github.com/germ-network/ATProtoLiteClient) | Lightweight AT Protocol client with OAuth | MIT | **Deprecated** (archived) |

## Rust packages

| Package | What it does | License | Status |
| --- | --- | --- | --- |
| [mls-rs-uniffi](https://github.com/germ-network/mls-rs-uniffi) | UniFFI wrapper over `mls-rs`, built as a `cdylib`/`staticlib` for iOS | MIT | Active |
| [TwoMLSPQ](https://github.com/germ-network/TwoMLSPQ) | `rust/` workspace behind the TwoMLSPQ Swift package. The crates set `publish = false` and are versioned by the repo's release tags, not independently | Apache-2.0 OR MIT | Active |

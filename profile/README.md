# CardanoWall

**Proof of Existence on Cardano — and the open standard behind it.**

Hash any content, anchor the digest on the Cardano blockchain, and later prove
that *this content existed on or before a given block time* — without trusting
our servers, our domain, or any issuer identity.

We authored and maintain **CIP-309**, the open standard for this, and publish
its complete reference implementation as open source. The standard is
issuer-agnostic and standalone-verifiable: any wallet can publish a proof, and
anyone can verify it from just the transaction and a public block explorer — no
issuer server required, ever.

## Open source

Licensed **Apache-2.0** (code) and **CC-BY-4.0** (the specification).

| Project | Package | What it is |
| --- | --- | --- |
| **[cip309](https://github.com/cardanowall/cip309)** | — | The standard: spec, CDDL, JSON Schemas, registries, conformance vectors |
| **[cip309-ts](https://github.com/cardanowall/cip309-ts)** | `@cardanowall/sdk-ts` · npm | TypeScript reference — primitives, wire format, SDK + standalone verifier |
| **[cip309-py](https://github.com/cardanowall/cip309-py)** | `cardanowall-sdk` · PyPI | Python SDK — byte-parity twin |
| **[cip309-rs](https://github.com/cardanowall/cip309-rs)** | `cardanowall` · crates.io | Rust SDK — byte-parity twin |
| **[cip309-cli](https://github.com/cardanowall/cip309-cli)** | `cardanowall-cli` · crates.io | Standalone CLI verifier + toolkit |

All three language SDKs are validated against the same canonical conformance
vectors and produce byte-identical output.

## Links

- 📖 **The standard:** [cip309.org](https://cip309.org)
- 🌐 **Hosted service:** [cardanowall.com](https://cardanowall.com)
- 📨 **Contact:** hello@cardanowall.com

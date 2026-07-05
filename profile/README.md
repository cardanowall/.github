# CardanoWall

**Proof of Existence on Cardano — and the open standard behind it.**

Hash any content, anchor the digest on the Cardano blockchain, and later prove
that *this content existed on or before a given block time* — without trusting
our servers, our domain, or any issuer identity.

We authored and maintain **Label 309**, the open standard for this, and publish
its complete reference implementation as open source. The standard is
issuer-agnostic and standalone-verifiable: any wallet can publish a proof, and
anyone can verify it from just the transaction and a public block explorer — no
issuer server required, ever.

## Open source

Licensed **Apache-2.0** (code) and **CC-BY-4.0** (the specification).

**The standard and its SDKs**

| Project | Packages | What it is |
| --- | --- | --- |
| **[label-309](https://github.com/cardanowall/label-309)** | — | The standard: spec, CDDL, JSON Schemas, registries, conformance vectors |
| **[label-309-ts](https://github.com/cardanowall/label-309-ts)** | `@cardanowall/crypto-core` · `@cardanowall/poe-standard` · `@cardanowall/sdk-ts` — npm | TypeScript reference: primitives, wire format, SDK + standalone verifier |
| **[label-309-py](https://github.com/cardanowall/label-309-py)** | `cardanowall-sdk` — PyPI | Python SDK — byte-parity twin |
| **[label-309-rs](https://github.com/cardanowall/label-309-rs)** | `cardanowall` — crates.io | Rust SDK — byte-parity twin |
| **[label-309-cli](https://github.com/cardanowall/label-309-cli)** | `cardanowall-cli` — crates.io | Command-line toolkit: publish, verify, seal, attest, and build/check Merkle proofs |

All three language SDKs are validated against the same canonical conformance
vectors and produce byte-identical output.

**Run it and wire it into CI**

| Project | What it is |
| --- | --- |
| **[label-309-gateway](https://github.com/cardanowall/label-309-gateway)** | The open-source gateway: transaction build, submit, confirm, Arweave storage, on-chain index, and pricing behind one binary + Postgres (`ghcr.io/cardanowall/label-309-gateway`) |
| **[poe-attest](https://github.com/cardanowall/poe-attest)** | GitHub Action — anchor a release's files, commit range, or precomputed digests as a Proof of Existence straight from CI (`uses: cardanowall/poe-attest@v1`) |
| **[poe-attest — GitLab](https://gitlab.com/cardanowall/poe-attest)** | The same tool as a GitLab CI/CD component (`include: component: gitlab.com/cardanowall/poe-attest/attest@1`) |

## Links

- 📖 **The standard:** [label309.org](https://label309.org)
- 🌐 **Hosted service:** [cardanowall.com](https://cardanowall.com)
- 📨 **Contact:** hello@cardanowall.com

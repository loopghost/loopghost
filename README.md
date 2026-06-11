# LoopGhost007

Data Science + Business student doing AI-driven Web3 security research.
I run autonomous auditing pipelines, then verify every finding with a reproducible PoC, no mocks.
Focus: zero-knowledge circuits, L1 consensus clients, and smart contracts.

### Selected disclosures

Every entry is publicly verifiable: each links to a merged fix, a published advisory, or a writeup.
Dates are the fix-merge or publication month.

| Date | Project | Severity | Vulnerability | Reference |
|------|---------|----------|---------------|-----------|
| 2026-06 | Payy Network | **Critical** | ZK circuit soundness: forged burn messages drain rollup USDC | [CVE-2026-48100](https://github.com/polybase/payy/security/advisories/GHSA-fhxc-63vg-9gwr) |
| 2026-03 | Polkadot SDK | **Critical** | XCM `fees` register not restored on rollback: permissionless asset duplication | [PR #11320](https://github.com/paritytech/polkadot-sdk/pull/11320) |
| 2026-03 | Celestia | **Critical** | `x/forwarding` collateral-token poisoning: permissionless TIA theft | [PR #6906](https://github.com/celestiaorg/celestia-app/pull/6906) |
| 2026-03 | Celestia | **Critical** | `x/forwarding` synthetic-slot poisoning: permanent TIA lock | [PR #6906](https://github.com/celestiaorg/celestia-app/pull/6906) |
| 2026-03 | Ripple xrpl-py | **Critical** (CVSS 9.3) | SField registry corruption: binary-codec crash and silent tx corruption | [PR #918](https://github.com/XRPLF/xrpl-py/pull/918) |
| 2026-02 | f(x) Protocol | **Critical** | FxUSD `wrapFrom` unbacked mint after pool liquidation | [commit](https://github.com/AladdinDAO/fx-protocol-contracts/commit/5e198e93657db008a57129e7eea21a996618f17f) |
| 2025-04 | Chainflip | **Critical** | AMM U256 overflow in `on_finalize`: consensus halt, ~$24M TVL frozen | [PR #5770](https://github.com/chainflip-io/chainflip-backend/pull/5770) |
| 2026-02 | Zircuit | Soundness (paid) | zkVM `l1_blocks` witness bypass: stale system-config in proven roots | [writeup](https://gist.github.com/loopghost/3ab50fb25cc0dcc00cf45ae5a3ec67ad) |
| 2026-04 | Ripple rippled | Medium | Invariant flag overwrite (`=` vs `\|=`): violations silently committed | [PR #6609](https://github.com/XRPLF/rippled/pull/6609) |

The Celestia fix ([PR #6906](https://github.com/celestiaorg/celestia-app/pull/6906)) credits `@loopghost` as reporter in the PR body.
Additional findings remain under private disclosure or embargo and are added here as fixes ship.

### Research areas
- Zero-knowledge proof systems: Noir, Halo2, circuit soundness
- L1 and consensus clients (Go, Rust, Scala): consensus halts, pre-auth DoS, runtime panics, state-machine safety
- EVM and non-EVM smart contracts: DeFi accounting, bridges, codec and invariant correctness

### Profiles
- Immunefi: [LoopGhost007](https://immunefi.com/profile/LoopGhost007/)
- HackenProof: [LoopGhost007](https://hackenproof.com/hackers/LoopGhost007)


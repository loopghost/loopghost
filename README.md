# LoopGhost007

Data Science + Business student doing AI-driven Web3 security research.
I run autonomous auditing pipelines, then verify every finding with a reproducible PoC, no mocks.
Focus: zero-knowledge circuits, L1 consensus clients, and smart contracts.

### Track record

Beyond the public CVE below, I have multiple additional High and Critical findings
reported through private bug bounty programs and direct vendor coordination. Public
writeups are added here as advisories are published and embargoes lift.

### Public disclosures

| Date | Target | Severity | Class | Reference |
|------|--------|----------|-------|-----------|
| 2026-06 | Payy Network (zk-rollup) | **Critical** | ZK circuit soundness | [CVE-2026-48100](https://github.com/polybase/payy/security/advisories/GHSA-fhxc-63vg-9gwr) |

**CVE-2026-48100: forged burn messages via an unconstrained `agg_agg` message tail.**
The recursive aggregation circuit copied only the active message prefix and never
zero-checked the unused tail of the public `messages` array, letting a registered
prover append a forged burn and drain USDC from the rollup contract. Reported and
credited as reporter; fixed in `beam-v0.1.0`.

### Research areas
- Zero-knowledge proof systems: Noir, Halo2, circuit soundness
- L1 and consensus clients (Go, Rust): pre-auth DoS, resource exhaustion, liveness and safety
- EVM and non-EVM smart contracts: DeFi accounting, bridges, access control

### Profiles
- Immunefi: [LoopGhost007](https://immunefi.com/profile/LoopGhost007/)
- HackenProof: [LoopGhost007](https://hackenproof.com/hackers/LoopGhost007)

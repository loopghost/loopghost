# Portfolio

Data Science + Business student doing AI-driven Web3 security research.
I run autonomous auditing pipelines.
Focus: zero-knowledge circuits, L1 consensus clients, and smart contracts.

### Selected disclosures

Every entry is publicly verifiable: each links to a merged fix, a published advisory, or a writeup.
Dates are the fix-merge or publication month.

| Date | Project | Severity | Vulnerability | Reference |
|------|---------|----------|---------------|-----------|
| 2026-06 | BitBox02 | **Critical** | BTC signing displays the attacker's `silent_payment` address instead of the device-derived multisig recipient (WYSIWYS): fund theft | [commit](https://github.com/BitBoxSwiss/bitbox02-firmware/commit/cbb40634cc24) |
| 2026-06 | BitBox02 | **Critical** | EIP-712 chainId queried twice without caching: device shows one chain, signs a digest bound to another (Permit2 cross-chain replay) | [commit](https://github.com/BitBoxSwiss/bitbox02-firmware/commit/cbb40634cc24) |
| 2026-06 | Payy Network | **Critical** | ZK circuit soundness: forged burn messages drain rollup USDC | [CVE-2026-48100](https://github.com/polybase/payy/security/advisories/GHSA-fhxc-63vg-9gwr) |
| 2026-05 | Trezor | **High** | Ethereum SLIP-24 verified-swap signs attacker calldata (guard `assert` stripped in production builds): Permit2/router drain | [advisory](https://trezor.io/vulnerability/ethereum-s-slip-24-payment-request-branch-in-production-firmware-signs-attacker-calldata-under-cover-of-verified-swap-ui) |
| 2026-04 | Ripple rippled | Medium | Invariant flag overwrite (`=` vs `\|=`): violations silently committed | [PR #6609](https://github.com/XRPLF/rippled/pull/6609) |
| 2026-04 | Polkadot SDK | **Critical** | Asset Hub `revive` precompiles miss `is_delegate_call()` guard: DELEGATECALL steals the caller's tokens and DOT | [PR #11676](https://github.com/paritytech/polkadot-sdk/pull/11676), [PR #11715](https://github.com/paritytech/polkadot-sdk/pull/11715) |
| 2026-04 | Trezor | **Critical** | Solana ALT-backed recipient spoofed on the signing screen: SOL and SPL theft | [advisory](https://trezor.io/vulnerability/solana-alt-recipient-confirmation-mismatch) |
| 2026-04 | Trezor | **Critical** | Solana account-type misclassification hides a CPI token drain in the blind-signing view | [advisory](https://trezor.io/vulnerability/solana-account-type-misclassification) |
| 2026-03 | Celestia | **Critical** | `x/forwarding` collateral-token poisoning: permissionless TIA theft | [PR #6906](https://github.com/celestiaorg/celestia-app/pull/6906) |
| 2026-03 | Celestia | **Critical** | `x/forwarding` synthetic-slot poisoning: permanent TIA lock | [PR #6906](https://github.com/celestiaorg/celestia-app/pull/6906) |
| 2026-03 | Polkadot SDK | **Critical** | XCM `fees` register not restored on rollback: permissionless asset duplication | [PR #11320](https://github.com/paritytech/polkadot-sdk/pull/11320) |
| 2026-03 | Ripple xrpl-py | **Critical** | SField registry corruption: binary-codec crash and silent tx corruption | [PR #918](https://github.com/XRPLF/xrpl-py/pull/918) |
| 2026-02 | f(x) Protocol | **Critical** | FxUSD `wrapFrom` unbacked mint after pool liquidation | [commit](https://github.com/AladdinDAO/fx-protocol-contracts/commit/5e198e93657db008a57129e7eea21a996618f17f) |
| 2026-02 | Zircuit | **Critical** | zkVM `l1_blocks` witness bypass: stale system-config in proven roots | [writeup](https://gist.github.com/loopghost/3ab50fb25cc0dcc00cf45ae5a3ec67ad) |
| 2026-02 | Chainflip | **Critical** | AMM U256 overflow in `on_finalize`: consensus halt, ~$24M TVL frozen | [commit](https://github.com/chainflip-io/chainflip-backend/commit/7cf98410161291e324e474657b2c918f7059f409) |

Additional findings remain under private disclosure or embargo and are added here as fixes ship.

### Research areas
- Zero-knowledge proof systems: Noir, Halo2, circuit soundness
- L1 and consensus clients (Go, Rust, Scala): consensus halts, pre-auth DoS, runtime panics, state-machine safety
- EVM and non-EVM smart contracts: DeFi accounting, bridges, codec and invariant correctness
- Hardware wallet signing-path integrity: transaction-display (WYSIWYS) and blind-signing bugs

### Profiles
- Immunefi: [LoopGhost007](https://immunefi.com/profile/LoopGhost007/)
- HackenProof: [LoopGhost007](https://hackenproof.com/hackers/LoopGhost007)

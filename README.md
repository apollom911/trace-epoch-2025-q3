# TRACE Epoch · Verification Rollup Capsule (Q3 2025)

**Release:** TRACE Epoch – 2025 Q3
“No staff. No supervisor. Just an army of one.”

---

## Latest Release
👉 [TRACE Epoch · Q3 2025 Rollup Capsule (v2025.3)](https://github.com/apollom911/trace-epoch-2025-q3/releases/tag/v2025.3)

All capsule artifacts (Rollup, Ledger, Exhibits A/B/D) are published as signed assets in the release.

---

## Repository Structure
- `/rollups/` — Rollup Capsule (Final PDF)  
- `/capsules/` — Ledger Capsule (SIM-01 → SIM-17)  
- `/exhibits/` — Hash Manifest, Domain Key Compression, Anchoring Note  
- `/validators/` — Independent attestations (open for PRs)

---

## Verify
1. Hash Exhibit A:
# macOS
shasum -a 256 exhibits/TRACE_EPOCH_2025_Q3_Exhibit_A_Hash_Manifest.txt

# Linux
sha256sum exhibits/TRACE_EPOCH_2025_Q3_Exhibit_A_Hash_Manifest.txt
2. Confirm it matches Exhibit D once TXID is posted.
3. Optionally recompute SIM payload hashes from the Ledger Capsule.

---

## Validators
1. Download assets from the [release](https://github.com/apollom911/trace-epoch-2025-q3/releases/tag/v2025.3).
2. Verify Exhibit A ↔ Exhibit D (anchored hash).
3. (Optional) Recompute SIM payload hashes.
4. Sign your attestation (PGP or minisign).
5. Submit via PR under `/validators/`.

---

## License
Documentation and exhibits © 2025 Rommel Wong.  
Released under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).

# Validators · TRACE Epoch Q3 2025

This folder is for independent validator attestations.

## How to Contribute
1. Download the [latest release](../releases/latest).
2. Verify Exhibit A ↔ Exhibit D (anchored hash).
3. (Optional) Recompute SIM payload hashes from the Ledger Capsule.
4. Sign your attestation with **PGP** or **minisign**.
5. Submit your signed attestation via Pull Request into this folder.

## Example
- `validator-attestation-alice.asc`
- `validator-attestation-bob.minisig`

## Notes
- Keep attestations in plain text (`.asc` or `.txt`) or minisign format (`.minisig`).
- Each attestation should include:
  - Manifest hash confirmation.
  - Optional recompute details.
  - Signature block.

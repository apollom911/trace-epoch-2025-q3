# Proofs Folder

This folder contains cryptographic proofs for the TRACE Epoch Q3 2025 publication.  
Each file here provides a different layer of verifiability:

---

## Files

- **TRACE_EPOCH_2025_Q3_Exhibit_A_Hash_Manifest.txt**  
  Human-readable manifest containing the SHA-256 digests of simulation payloads (SIM-01 … SIM-17).  
  Serves as the canonical reference for what was hashed.  
  - Manifest checksum (file-level SHA-256):  
    `c54193afb02734e14b9d2ad651515792d0800eec470c761c00cc179d4ea70ef3`

- **TRACE_EPOCH_2025_Q3_Exhibit_D_Anchoring_Note.txt**  
  Anchoring note linking Exhibit A’s manifest checksum into the TRACE Epoch Q3 2025 publication.  
  Confirms anchoring context, attestation servers, and integrity status.  
  - Anchored manifest hash:  
    `c54193afb02734e14b9d2ad651515792d0800eec470c761c00cc179d4ea70ef3`

- **TRACE_EPOCH_2025_Q3_Exhibit_A_Hash_Manifest.txt.ots**  
  OpenTimestamps receipt corresponding to Exhibit A manifest file.  
  This proves the manifest file itself (`Exhibit_A_Hash_Manifest.txt`) existed at the recorded time.  
  - OTS file-level SHA-256:  
    `e7341879d8a24f3807633e1b9fcf3647105d4ce693995b07fe6c9cba566xxxx`  
  - Verification can be performed at [opentimestamps.org](https://opentimestamps.org).

---

## Verification Steps

1. **Manifest Integrity**  
   Compare hashes listed in `Exhibit_A_Hash_Manifest.txt` against simulation payloads.  
   The manifest checksum is: c54193afb02734e14b9d2ad651515792d0800eec470c761c00cc179d4ea70ef3

2. **Anchoring Integrity**  
Confirm that `Exhibit_D_Anchoring_Note.txt` records the same manifest checksum.  
Match = Yes.

3. **Timestamp Proof**  
Verify `TRACE_EPOCH_2025_Q3_Exhibit_A_Hash_Manifest.txt.ots` using [OpenTimestamps](https://opentimestamps.org).  
This proves the manifest file existed at the anchored time, independent of TRACE Epoch.

---

## Summary

- **Exhibit A** defines the canonical SHA-256 digests of simulation payloads.  
- **Exhibit D** anchors Exhibit A’s checksum into TRACE Epoch Q3 2025.  
- **OTS receipt** cryptographically timestamps the Exhibit A file itself.  

Together these provide **end-to-end integrity, anchoring, and timestamp verification**.

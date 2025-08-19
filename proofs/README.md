# Proofs Folder

This folder contains cryptographic proofs for the TRACE Epoch 2025 Q3 capsule.  

## Files

- **TRACE_EPOCH_2025_Q3_Exhibit_A_Hash_Manifest.txt**  
  Human-readable manifest containing the SHA-256 digest of Exhibit A payloads.  
  Serves as the canonical reference for what was hashed.

- **TRACE_EPOCH_2025_Q3_Exhibit_A_Hash_Manifest.txt.ots**  
  OpenTimestamps receipt corresponding to the manifest.  
  This file proves that the manifest hash existed prior to the attested Bitcoin block timestamp.  
  Verification can be performed at [opentimestamps.org](https://opentimestamps.org).

## Usage

1. To verify the proof, upload the `.ots` file along with the manifest to the OpenTimestamps verifier.  
2. The verifier will check inclusion against the Bitcoin blockchain.  
3. Once confirmed, this provides immutable anchoring for Exhibit A.

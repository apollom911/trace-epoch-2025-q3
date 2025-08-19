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

## Usage (Web)

1. Go to [opentimestamps.org](https://opentimestamps.org).  
2. Upload the `.ots` file and the `TRACE_EPOCH_2025_Q3_Exhibit_A_Hash_Manifest.txt`.  
3. The verifier will confirm inclusion against the Bitcoin blockchain.  
4. Once confirmed, this provides immutable anchoring for Exhibit A.

## Usage (Command Line)

If you have the `opentimestamps-client` installed:

```bash
# Verify the timestamp against the Bitcoin blockchain
ots verify TRACE_EPOCH_2025_Q3_Exhibit_A_Hash_Manifest.txt.ots \
           TRACE_EPOCH_2025_Q3_Exhibit_A_Hash_Manifest.txt

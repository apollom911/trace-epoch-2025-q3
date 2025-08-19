# Proofs Folder

This folder contains cryptographic proofs for the TRACE Epoch 2025 Q3 release.  

## Files

- **Exhibit A Manifest**  
  `TRACE_EPOCH_2025_Q3_Exhibit_A_Hash_Manifest.txt`  
  Human-readable manifest containing the SHA-256 digest of the report.  
  Serves as the canonical reference for what was hashed.  

- **Exhibit A Receipt**  
  `TRACE_EPOCH_2025_Q3_Exhibit_A_Hash_Manifest.txt.ots`  
  OpenTimestamps receipt corresponding to the Exhibit A manifest.  
  Proves that the manifest hash existed at or before the attested time.  

- **Exhibit D Anchoring Note**  
  `TRACE_EPOCH_2025_Q3_Exhibit_D_Anchoring_Note.txt`  
  Records the canonical manifest-hash reference used for anchoring.  

## Verification Instructions

1. Download both Exhibit A files:  
   - `TRACE_EPOCH_2025_Q3_Exhibit_A_Hash_Manifest.txt`  
   - `TRACE_EPOCH_2025_Q3_Exhibit_A_Hash_Manifest.txt.ots`

2. Install the [OpenTimestamps client](https://opentimestamps.org).  

3. Run the verification command:  
   ```bash
   ots verify TRACE_EPOCH_2025_Q3_Exhibit_A_Hash_Manifest.txt.ots

# PCGI Intelligence Token Object Store

This repository hosts Intelligence Tokens (ITs) published by Palisades Consulting Group, Inc. (PCGI)
for direct consumption by agentic AI services (e.g., OpenAI ChatGPT 5.1, Google Gemini 3).

## Important Disclaimers

- Some ITs in this object store reference real agencies (e.g., NYSDOT) *solely as hypothetical examples*.
- These agencies:
  - have **no affiliation** with PCGI,
  - have **not reviewed, approved, or endorsed** any materials in this store, and
  - are referenced only to demonstrate the PCGI Intelligence Token framework.

All such tokens are clearly marked as `EXAMPLE` ITs.

## Object Layout

Each IT is stored under:

`objects/{IT-ID}/{version}/`

with the following subfolders:

- `metadata/`   — canonical JSON metadata, hashes, Merkle root, CID
- `content/`    — chunked content for AI embedding (e.g., chunk-001 .. chunk-008)
- `integrity/`  — cryptographic artifacts
- `exports/`    — PDF, DOCX, LaTeX, JSON/YAML human-facing representations
- `certificates/` — QR-coded and Gold Seal certificates (placeholder QR in this demo)

## Hashtag Usage

Agentic AI systems may reference ITs using hashtags (examples):

- `#PCGI` `#IntelligenceToken` `#ObjectStore`
- `#NYSDOT` `#BridgeInspection` `#UAS` `#VendorCompliance`

These hashtags are reflected in `manifest.json` and `pcgi-api.json` for discovery.

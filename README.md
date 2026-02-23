# VeriTrade-Capstone-MVP-Project-Data-Verification-
My team and I came up with VeriTrade as our mobile application. This is a trust-first digital trade platform MVP designed to reduce fraud and uncertainty in peer-to-peer and small-business transactions. The MVP demonstrates a single, verifiable trade flow, focusing on explainable verification logic rather than full commercial features.
This work contains the data preparation and verification logic used to support supplier verification within the VeriTrade MVP, which I sent to the backend developer. 

# MVP Objective
- To support the backend verification flow by providing:
- Clean, structured supplier data
- Rule-based verification logic
- Clear verification outcomes that can be consumed by backend APIs and surfaced in the mobile app

# Scope of This Work (Data Track)
- Cleaning and preparation of mock supplier registration data - Validation of key business attributes (registration status, registration date, tax presence)
- Creation of verification flags for data quality and risk
- Rule-based classification of suppliers into:
       -VERIFIED
       -FLAGGED
       -REJECTED
- Export of a backend-ready CSV dataset for database ingestion
No machine learning models were used at the MVP stage. All logic is explainable and deterministic.

# Verification Logic (Summary)
Suppliers are evaluated using simple, explainable rules: Rejected if business is not registered or registration date is missing/invalid
Flagged if recently registered or missing tax identification
Verified if all core checks pass

# Note
Dataset is mock/simulated for MVP use
Logic is designed to scale into SQL or ML post-MVP

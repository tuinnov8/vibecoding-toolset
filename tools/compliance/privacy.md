# Data Privacy & Compliance (GDPR/CCPA)

1. **No PII Logging:** Never log Personally Identifiable Information (PII) such as emails, names, or passwords to the console or log files.
2. **Data Masking:** Mask PII in all database outputs and debug traces.
3. **Password Security:** Always hash passwords (e.g., using bcrypt or Argon2) before saving to the database. Never transmit plain-text passwords over unencrypted connections.

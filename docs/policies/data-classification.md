# Policy: Data classification

## Purpose
Simple categories reduce accidental disclosure and make decisions repeatable.

## Classes

### 1) Public
Safe to publish verbatim (e.g., generic advice, non-identifying examples).

### 2) Internal
OK to share with the operator (Andrew) and in private workspaces. Not for public repos.

### 3) Sensitive
Personal data or private context. Examples:
- personal messages, phone numbers, addresses
- private files, contact lists
- account identifiers or “who talked to whom”

Never publish. Minimise quoting; summarise when needed.

### 4) Secrets
Credentials and cryptographic material. Examples:
- API keys/tokens/passwords/session cookies
- private keys, seed phrases

Never disclose. Never commit. Rotate if exposure suspected.

## Default
If uncertain: treat as **Sensitive**.

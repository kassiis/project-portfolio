# PassGuard

**GitHub Repository:** `kassiis/passguard` 
**Source code:** Private repository  
**public code:** 'https://github.com/kassiis/passguard-service'
**Project Category:** Cybersecurity & Security Microservices  
**Development Status:** Active / Feature-Complete Prototype  

---

## 1. Overview

**PassGuard** is a modular password security microservice and authentication utility designed to enforce modern cryptographic best practices. It provides automated password strength analysis, high-entropy credential generation, RFC-compliant time-based one-time password (TOTP) two-factor authentication, and privacy-preserving breached credential verification.

---

## 2. Project Purpose

Authentication vulnerabilities remain a primary entry point in enterprise and web applications. PassGuard was engineered to centralize and standardize credential security policies into a decoupled service, enabling applications to:

- Quantify password resistance against dictionary and brute-force attacks prior to storage.
- Provide users with cryptographically sound passwords and Diceware passphrases.
- Protect accounts via standards-compliant two-factor authentication.
- Safely check passwords against known global breach corpuses without disclosing the plaintext or full hash.

---

## 3. Key Capabilities

- **Entropy & Strength Evaluation:** Multi-criteria analysis examining character composition, length, structural patterns, and checking against extensive dictionary lists of common passwords.
- **CSPRNG Password Generation:** Generation of high-entropy credentials utilizing cryptographically secure pseudorandom number generators.
- **Diceware Passphrase Generation:** Generation of memorable, high-entropy multi-word passphrases using established Electronic Frontier Foundation (EFF) wordlist standards.
- **Standards-Compliant TOTP (RFC 6238):** Full lifecycle management for time-based one-time passwords, including shared secret generation, URI QR-compatibility formatting, and time-drift verification windows.
- **Privacy-Preserving Breach Verification:** Integration of the Have I Been Pwned k-anonymity API model, querying breached credential databases using a 5-character SHA-1 prefix without transmitting sensitive full hashes or plaintext.
- **Modern Key Derivation:** Argon2id password hashing implementation, providing resistance against GPU- and ASIC-accelerated cracking attacks.
- **RESTful Service Architecture:** Clean HTTP API endpoints with configurable header-based authentication guards.

---

## 4. Technologies Used

- **Language:** Python 3
- **Framework:** Flask (RESTful Microservice Architecture)
- **Cryptography & Security:** Argon2 (Argon2id KDF), PyOTP (RFC 6238 TOTP), `secrets` (CSPRNG)
- **HTTP Client:** Requests
- **Testing & Quality Assurance:** pytest (comprehensive test coverage across entropy, generation, and API layers)

---

[← Return to Project Portfolio](../README.md)

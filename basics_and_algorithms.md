# Cryptography Basics — Symmetric vs Asymmetric, Hashing, Certificates

## Symmetric Encryption
- Single shared key for encryption & decryption (AES, 3DES).
- Fast, good for bulk data encryption.
- Key distribution is a challenge.

## Asymmetric Encryption
- Public/private key pairs (RSA, ECC).
- Public key encrypts, private key decrypts (or signs).
- Used for key exchange, digital signatures, small payloads.

## Hashing
- One-way functions: MD5 (deprecated), SHA-1 (weak), SHA-256, SHA-3.
- Use cases: integrity checks, password hashing (with salt and KDF like bcrypt/argon2).
- Collision resistance and preimage resistance are important properties.

## Digital Certificates & SSL/TLS
- X.509 certificates bind an identity to a public key.
- Certificate chain: leaf -> intermediates -> root CA.
- Certificate issuance often involves CSR (Certificate Signing Request).
- Revocation: CRL or OCSP.

## OpenSSL hands-on (encrypt/decrypt text)
- Generate RSA private key:
  `openssl genpkey -algorithm RSA -out private.pem -pkeyopt rsa_keygen_bits:2048`
- Extract public key:
  `openssl rsa -in private.pem -pubout -out public.pem`
- Encrypt with public key:
  `echo "secret message" > msg.txt`
  `openssl rsautl -encrypt -inkey public.pem -pubin -in msg.txt -out msg.enc`
- Decrypt with private key:
  `openssl rsautl -decrypt -inkey private.pem -in msg.enc`
- Symmetric encryption (AES):
  `openssl enc -aes-256-cbc -salt -in plaintext.txt -out ciphertext.bin`
  `openssl enc -d -aes-256-cbc -in ciphertext.bin -out plaintext.txt`
- Hashing examples:
  `echo -n "data" | openssl dgst -sha256`
  `echo -n "data" | md5sum`  # md5 for legacy only

## Notes
- Do not use MD5 or SHA-1 for security-critical needs.
- For passwords use bcrypt, scrypt, or Argon2 with salts.

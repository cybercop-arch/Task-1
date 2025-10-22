# The CIA Triad — Confidentiality, Integrity, Availability

The CIA Triad is a foundational model in information security composed of three core principles:

## Confidentiality
- Ensures information is accessible only to authorized individuals/systems.
- Controls: Access control (RBAC, ABAC), encryption (at-rest and in-transit), strong authentication, data classification.
- Examples: Using TLS for web traffic, AES for disk encryption, least privilege policies.

## Integrity
- Ensures data remains accurate and unaltered except by authorized actions.
- Controls: Checksums, cryptographic hashes (SHA-2/3), digital signatures, versioning, secure logging, input validation.
- Examples: Git commit hashes, signed software packages, database constraints and transactions.

## Availability
- Ensures systems and data are available when needed by authorized users.
- Controls: Redundancy, backups, failover, DDoS protection, SLAs, patch management, monitoring and alerting.
- Examples: RAID, load balancers, regular backups, high-availability clusters.

## Balancing the Triad
- Security controls often trade off across the triad (e.g., stronger confidentiality may reduce availability if access is blocked).
- Use risk assessments and business impact analysis (BIA) to prioritize.

## Quick checklist
- Is sensitive data encrypted at rest & in transit?
- Are access controls and MFA in place?
- Do backups exist and are they tested?
- Are integrity checks or logs protected from tampering?

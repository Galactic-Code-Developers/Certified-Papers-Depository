# 📄 Certified Scientific Paper Repository

This repository contains officially **signed, verified scientific papers** issued by the **Kapodistrian Academy of Science**. Each document is digitally certified and tamper-evident through embedded SHA-256 cryptographic hashes, structured metadata, and a formal audit trail.

---

## ✅ Repository Purpose

- 🔏 Ensure **authenticity** and **integrity** of scientific publications.
- 🧾 Maintain a verifiable audit trail for each signed release.
- 📚 Provide researchers, reviewers, and institutions with **trusted, immutable access** to certified documents.

---

## 🧬 Document Integrity Features

Each scientific paper in this repository is accompanied by:

- A `.pdf` file with:
  - A **SHA-256 cryptographic hash** embedded visibly in the last-page footer.
  - The signer's initials and signing **UTC timestamp**.
  - Fully embedded PDF **metadata** (author, ORCID, institution, email, version).
- A `.sha256` file containing the raw hash value for independent verification.
- A `.meta.txt` file detailing all human-readable metadata fields.
- An appended entry in `KAS_audit.log`, preserving the full certification record.

---

## 📂 Repository Structure

```plaintext
Certified_Papers/
├── YourPaper_v1.0_SIGNED_KAS_2025-05-09.pdf
├── YourPaper_v1.0_SIGNED_KAS_2025-05-09.sha256
├── YourPaper_v1.0_SIGNED_KAS_2025-05-09.meta.txt
├── KAS_audit.log

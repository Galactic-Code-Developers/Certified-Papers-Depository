# 📄 Certified Scientific Paper Repository

This repository contains officially **signed, verified scientific papers** issued by the **Kapodistrian Academy of Science**. Each document is digitally certified and tamper-evident through embedded SHA-256 cryptographic hashes and audit metadata.

---

## ✅ Repository Purpose

- 🔏 Ensure **authenticity** and **integrity** of scientific publications.
- 🧾 Maintain a verifiable audit trail for each signed release.
- 📚 Provide researchers and institutions with **trusted, immutable access** to certified documents.

---

## 🧬 Document Integrity

Each `.pdf` in this repository has:

- A **cryptographic SHA-256 hash** embedded in the footer.
- A **timestamp** and digital signer ID.
- Embedded **metadata** (author, institution, ORCID, version, etc.).
- A corresponding `.sha256` and `.meta.txt` file for independent validation.
- An audit log entry stored in `KAS_audit.log`.

---

## 📂 File Structure

```plaintext
[year]{month}/
├── Paper_Title_v1.2_SIGNED_KAS_2025-05-09.pdf
├── Paper_Title_v1.2_SIGNED_KAS_2025-05-09.sha256
├── Paper_Title_v1.2_SIGNED_KAS_2025-05-09.meta.txt
├── KAS_audit.log
```

---

## 🛡️ Verification Instructions

Open the PDF file.  
Scroll to the last page to find the embedded SHA-256 hash, timestamp, and signer ID.

**Match the hash.**  
Compare the hash shown in the PDF with the one in the `.sha256` file using any SHA-256 tool.

**Review metadata.**  
Open the `.meta.txt` file to confirm authorship, ORCID, institutional affiliation, and declared version.

**Cross-check audit log.**  
Look inside `KAS_audit.log` for the certified entry corresponding to the paper’s filename.

---

## 🔧 Technical Notes

- Hashes are generated using `hashlib.sha256` in Python.
- Footer content is injected using PyMuPDF (`fitz`) with a monospaced font (`courier`) for clarity.
- The last-page textbox is carefully sized to prevent overflow or wrapping of the SHA-256 string.

---

## 🏛️ Issuing Authority

Kapodistrian Academy of Science  
Scientific Certification Program  
🌐 [kapodistrian.edu.gr](https://kapodistrian.edu.gr)  
✉️ validation@kapodistrian.edu.gr

---

## 📜 License

All certified works remain under the copyright and distribution terms  
as stated by the original authors. This repository guarantees their  
**authenticity**, not their licensing terms.

For questions regarding usage, please contact the corresponding author listed in each `.meta.txt` file.

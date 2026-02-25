# 🏛️ Tallo CPA | Certificate Authentication Registry

Welcome to the **Official Certificate Verification System** for Tallo CPA. This repository serves as the public "Source of Truth" for authenticating audit certificates issued by our firm.

## 🛡️ Purpose
This registry allows clients, banks, and regulatory bodies to verify that an audit certificate in their possession is authentic and has not been tampered with. Every official document we issue contains a unique QR code that points directly to this secure database.

## 🔍 How to Verify
1. **Scan the QR Code** on the physical certificate.
2. You will be redirected to our secure verification page: `https://[your-username].github.io/audit-verify/`
3. Ensure the **Certificate ID**, **Client Name**, and **Audit Year** displayed on your screen exactly match the physical document.

---

## ⚙️ System Workflow (Internal Use Only)
This system is automated using **Google Workspace** and **GitHub Pages**.

1. **Submission:** Audit details are entered via a private Google Form.
2. **Review:** Data is checked in the Google Sheets response tab.
3. **Approval:** A firm administrator clicks the "Approved" checkbox.
4. **Generation:** 
   - A Google Doc is created in the `Processed Certificates` folder.
   - A secure PDF is generated in the `Generated Certificates` folder.
   - The unique Certificate ID is pushed to this GitHub repository's `database.json`.
5. **Verification:** The public-facing `index.html` reads the database to confirm authenticity.

## 🛠️ Tech Stack
- **Google Apps Script:** The engine for document generation and API sync.
- **GitHub Pages:** Hosting for the public verification portal.
- **JSON:** Lightweight database for certificate records.

---

## ⚖️ Legal Disclaimer
The information provided by this verification service is intended solely for the purpose of confirming the authenticity of documents issued by **Tallo CPA**. 
- This portal does not provide financial, tax, or legal advice. 
- Receipt of a "Verified" status does not constitute a new accountant-client relationship.
- Tallo CPA assumes no liability for decisions made based on this verification tool without direct consultation with our professional staff.

---

[Return to Tallo CPA Homepage](https://www.tallocpa.com)
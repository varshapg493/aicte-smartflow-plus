# AICTE SmartFlow Plus — Full-stack prototype

A colourful SIH demonstration prototype with six feature areas:
1. Automated preliminary validation of required fields, contact email, deadlines and document checklist.
2. Reviewer scrutiny: update status, mark documents, record deficiencies, and view review history.
3. Student complaint portal with status tracking and evidence uploads (PDF, PNG, JPG/JPEG; up to 5 MB per file).
4. Centralized overview with application, review, overdue, missing-document and complaint metrics.
5. Application change intelligence using a timestamped field-level audit trail and re-validation.
6. Requirement impact analysis with illustrative dependency maps.

## Run locally
Requires Node.js 18 or newer.

```bash
npm install
npm start
```

Open http://localhost:5000

## Storage and safety notes
- Demo records are stored in `data/applications.json` and `data/complaints.json`; evidence files are in `uploads/`.
- Local JSON storage and uploaded files may not persist on ephemeral hosting such as a free web service. Use a managed database/object storage for reliable hosted persistence.
- This is a prototype, not an official AICTE integration. Sample records are fictional. Validation and requirement dependencies are illustrative and must be checked against the current official process. Do not upload real sensitive student data.
- Evidence upload filtering checks file extension and size, not file contents. Do not use for production without authentication, authorization, stronger file validation, malware scanning, privacy controls and secure persistent storage.

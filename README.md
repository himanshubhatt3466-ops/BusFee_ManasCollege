# Manas College Pithoragarh — Bus Fee Manager

A browser-based starter application for registering bus students, buses, bus stops and monthly fees.

## Run locally
1. Download and extract this folder.
2. Double-click `index.html` to open it in Chrome or Edge.
3. Data is stored in the browser on that computer. Use **Export backup** regularly.

No local Node.js installation is required.

## Publish with GitHub Pages
1. Create a GitHub repository, e.g. `manas-college-bus-fees`.
2. Upload `index.html` and this README to the repository root.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Choose branch `main`, folder `/ (root)`, and save.
6. Wait for GitHub Pages to publish the site.

## Included
- Dashboard cards and charts for buses, students, collections, pending fees and fines.
- Student registration with ID card number, name, gender, bus, stop, course, semester and mobile.
- Add/edit buses and stops, with a separate monthly fee for each stop.
- Fee payments by cash, UPI, online, internet banking, card, cheque or other.
- Advance payment across multiple months.
- Student search and month-wise fee history.
- Month skip option.
- Printable receipt / Save as PDF, with optional college logo and authorized signature.
- JSON export/import backup.

## Important limitations before real college use
- **This starter stores data in browser local storage.** It is not a shared multi-user database. Data does not automatically sync across computers or browsers.
- **Google Cloud daily backup is not active in this static starter.** GitHub Pages cannot read a local browser database on a schedule. For genuine automatic daily backups, connect a cloud database (for example, Firestore) and configure a secure scheduled server-side backup using Google Cloud credentials. Never put service-account keys in `index.html` or commit them to GitHub.
- The fine calculation is a simple estimate: after the configured day, the daily fine is added while the month remains unpaid. Confirm the exact college policy (including whether fine is capped and how partial payments affect it) before using it for official accounts.
- Payment allocation and receipts are an operational starter, not an audited accounting system. Test with sample data and reconcile receipts before real fee collection.
- Logo and signature images are optional and are stored in this browser's data. Upload only an approved college logo and authorized signature.
- Export backups contain student personal data. Store them securely and limit access.

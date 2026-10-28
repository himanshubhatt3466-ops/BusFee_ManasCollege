# Manas College Bus Fee Manager — Windows EXE

This repository builds a Windows desktop application from the included `index.html`. It includes the MCSTM college logo in the receipt and shows month names such as **October 2026**. The dashboard shows the supplied MCSTM college logo. The current fee logic applies a **one-time ₹100 fine per unpaid month after the 10th**, not ₹100 per day. In Fee Payments, select a student and month, then use **Mark selected month skipped** or **Undo skipped / Restore fee**; the status is saved immediately.

## No Node.js needed on your computer

The EXE is built by GitHub Actions on GitHub's Windows runner. You do not need to install Node.js locally.

## Build the EXE on GitHub

1. Create a new GitHub repository, for example `ManasCollegeBusFees`.
2. Upload **all files and folders** from this project to the repository root. Make sure `.github/workflows/build-windows.yml` is included.
3. Open the repository's **Actions** tab.
4. If prompted, enable GitHub Actions.
5. Select **Build Windows EXE** → **Run workflow** → **Run workflow**.
6. Wait until the workflow is green/successful.
7. Open the completed workflow run and scroll to **Artifacts**.
8. Download **ManasCollegeBusFees-Windows** and extract the ZIP.
9. Run the `Manas College Bus Fee Manager Setup ... .exe` installer, or run the portable `.exe`.

## Make a GitHub Release (optional)

After uploading the project and getting a successful build, create and push a tag named `v1.0.0` (GitHub website: Releases → Draft a new release → tag `v1.0.0`). The workflow builds the EXEs and attaches them to the release. You can then download the installer from the repository's Releases page.

## Important notes

- The app stores data in the local app/browser storage on that Windows user profile. This starter does not sync records between multiple computers and does not yet set up Google Cloud backups.
- Export backups from the app regularly and store them securely.
- Test the fine and skipped-month rules with sample students before using the app for official accounts.
- Never upload private student records or secrets to a public GitHub repository.
- GitHub Actions installs Electron/build tools on GitHub's own runner; nothing needs to be installed on your local PC to build the EXE.

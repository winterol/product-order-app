PRODUCT ORDER — GITHUB PAGES INSTALLABLE SHELL PROTOTYPE

Files: index.html, manifest.webmanifest, icon-192.png, icon-512.png.

This prototype provides a manifest and custom icons for GitHub Pages. It is only a launcher: the current Apps Script app uses google.script.run, which is only available inside Apps Script HTMLService. GitHub Pages cannot run that API directly, and this prototype intentionally does not embed or modify the live app. The Open Product Order button opens the existing deployment.

Before staff use, a separate integration design is required if the actual app UI must run inside the installable PWA. Do not change the existing deployment yet.

Password policy files are separate: App_4Digit_PIN.html and CloudBackend_4Digit_PIN.gs. They have not been deployed or tested against the live spreadsheet. The backend change supports new/change PINs of exactly four digits; existing hashes are not migrated and existing credentials continue to verify as before. Four-digit PINs have only 10,000 combinations and are weak for customer/financial data. Use only if you accept that risk.

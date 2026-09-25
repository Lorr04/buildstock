BUILDSTOCK — MATERIAL INVENTORY MANAGEMENT SYSTEM
Fixed classroom prototype — September 2026

LOGIN
Username: admin
Password: admin123

IMPORTANT FIX
The previous version used browser-generated element variables such as f_id and f_name. Those variables are not guaranteed to exist when the form is created dynamically, so Save buttons could appear to do nothing. This version reads every form field with document.getElementById(), validates the data, saves it to localStorage, updates the tables, and writes an audit event.

FUNCTIONS TESTED
✓ Login
✓ Add Material
✓ Add Supplier
✓ Record Delivery
✓ Issue Material
✓ Record Return
✓ Automatic inventory update
✓ Search/filter
✓ Reports and CSV export
✓ Audit trail
✓ Local browser storage

GITHUB PAGES
1. Open the BuildStock folder inside this ZIP.
2. Upload INDEX.HTML (exactly lowercase: index.html) to the ROOT of your GitHub repository.
3. If you also have other files, keep them beside index.html. Do not put index.html inside another folder unless Pages is configured to publish that folder.
4. Settings → Pages → Deploy from a branch → main → / (root).
5. Open the generated Pages link after GitHub finishes deploying.

DATA NOTE
This is a browser-based classroom prototype. Each computer/browser has its own localStorage. Adding a material on one groupmate's computer will not automatically appear on another computer. A shared multi-user version would require an online database/backend.

RESET DEMO DATA
If you need the original sample dataset again, clear the site's localStorage for BuildStock and reload the page. The system will recreate the sample records.

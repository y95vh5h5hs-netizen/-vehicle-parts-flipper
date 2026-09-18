VEHICLE PARTS FLIPPER V1.1

Replace the old files in your GitHub repository with these files.

Changes:
- Year is a dropdown.
- Make is a searchable dropdown populated from NHTSA vPIC.
- Model is a searchable dropdown filtered by Year + Make for 1996+ vehicles.
- eBay Research uses a real HTTPS link instead of window.open, so Firefox popup blocking does not prevent it from working.
- The app loads parts.json at startup.
- A GitHub Action uses Playwright to open Carolina Pick-N-Pull's official price page, click All, and extract the complete table into parts.json.
- The Action runs weekly and can also be run manually.
- The Action refuses to overwrite parts.json if fewer than 100 rows are found.

After uploading:
1. Commit the files.
2. Open GitHub -> Actions.
3. Select "Update Carolina Pick-N-Pull Price List".
4. Tap "Run workflow".
5. Wait for it to finish successfully.
6. Refresh the GitHub Pages site in Firefox.

The live Carolina page currently exposes the A-Z selector and All option. The web text retrieval only exposes the A-section, so the browser-based Action is used to obtain the complete All table rather than inventing B-Z prices.

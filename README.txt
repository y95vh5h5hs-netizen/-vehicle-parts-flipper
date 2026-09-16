VEHICLE PARTS FLIPPER — VERSION 1 PWA

This build is a real installable web-app package. It is designed to be hosted at a normal HTTPS web address, then added to the iPhone Home Screen.

IMPORTANT:
The iPhone Files app cannot turn an HTML file into an installed web app. For the "Add to Home Screen" experience, the files need to be served from an HTTPS web address.

FREE SETUP OPTION (GitHub Pages):
1. Create a free GitHub account if you don't already have one.
2. Create a new public repository named vehicle-parts-flipper.
3. Upload ALL files in this folder to the repository root:
   index.html
   manifest.webmanifest
   sw.js
   icon-192.png
   icon-512.png
4. In GitHub: Settings -> Pages -> Deploy from branch -> main -> / (root) -> Save.
5. GitHub will provide an HTTPS Pages URL.
6. Open that URL in Safari on the iPhone.
7. Tap Share -> Add to Home Screen -> Add.

The app then works as a standalone Home Screen web app and caches the app shell for offline use.

V1 E-BAY WORKFLOW:
- The app does NOT scrape eBay.
- Tap "eBay Product Research" or "Research on eBay".
- Use the official Product Research tool, set the date range to the last 30 days, and apply appropriate used/vehicle-part filters.
- Enter the sold statistics into the app.
- The app calculates estimated net profit, ROI, and maximum acquisition price.

CAROLINA PICK-N-PULL:
- Tap "Carolina Price List" to open the current official price list.
- The app treats core charges separately because Carolina says eligible core charges may be refunded when returned to the purchasing store within 30 days with the original dated receipt.
- The official price list should remain the source of truth because prices can change.
- The current web retrieval available to the builder exposed the A section of the table; the site's A-Z controls did not expose the other letter contents to the retrieval layer. Therefore this build does not falsely claim to contain an entire verified A-Z price database. You can add any missing part with the "+ Add part" button.

PROFIT SETTINGS:
- eBay fee percentage
- Packaging
- Desired profit
- Shipping
- Median/average/custom sale-price basis

This is a free personal-use tool and does not require a paid server or API.

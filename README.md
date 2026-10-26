# Koyava Smart Restaurant — QR Ordering Demo

## What's included
- Mobile-friendly restaurant menu, category filters and search
- Cart with quantities and totals
- Checkout form: name, phone, optional email, table/takeaway and notes
- Orders/customer records stored in this browser's localStorage
- Review form and reviews list
- Demo admin dashboard with Orders, Customers, Menu and Reviews tabs
- Export demo data to JSON
- QR-ready: after hosting, create a QR code for the public website URL

## Important limits
This is a **front-end demo**, not production software. Data is stored in the current browser/device only; it is not shared between customer phones and the restaurant owner's admin panel. There is no real server/database, admin login, payment processing, live kitchen notification or WhatsApp automation. Do not use this demo for real customer data or actual restaurant operations.

## Test locally
Open `index.html` in a modern browser. If the browser blocks local files, use a simple static local server or upload the folder to a static hosting provider.

## Publish free with GitHub Pages (mobile steps may be easier on a laptop)
1. Sign in or create a GitHub account at https://github.com/
2. Create a new public repository named `koyava-restaurant-qr`.
3. Upload `index.html`, `style.css`, and `app.js` to the repository root (not inside another folder).
4. Open repository **Settings → Pages**.
5. Under Build and deployment, select **Deploy from a branch**.
6. Choose branch `main`, folder `/ (root)`, then Save.
7. Wait for GitHub Pages to publish. The URL normally looks like `https://YOUR-USERNAME.github.io/koyava-restaurant-qr/`.
8. Open the public URL on your phone and test menu, cart, checkout, review and Admin.
9. Generate a QR code that points to the public URL. For table-specific QR codes, add a URL parameter such as `?table=4`; this demo does not yet read that parameter automatically.

## To turn this into a real client-ready system
You will need:
- A shared backend database (e.g. Supabase free tier, subject to its current limits)
- Secure admin authentication and access rules
- Server-side order creation and validation
- Privacy notice and consent for customer data
- WhatsApp Business Platform/API integration for automatic reminders; costs and template rules may apply
- A deployment configuration and testing for the chosen backend

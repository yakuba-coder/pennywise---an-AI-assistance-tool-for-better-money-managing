# Pennywise — No-AI Static Dashboard

Pennywise is a browser-based personal finance dashboard. This build removes the AI integration and server/backend files. Transaction parsing, budgets, savings goals, charts, insights, recurring-payment estimates, and report generation run in the browser. Dashboard data is stored in this browser's localStorage.

## Deploy to Vercel
1. Upload the **contents** of this folder directly to the root of a GitHub repository.
2. Import the repository in Vercel.
3. Set Framework Preset to **Other**.
4. Set Root Directory to the repository root.
5. Leave Build Command, Output Directory, and Install Command overrides disabled/empty (use defaults).
6. Deploy. No API key, build step, npm install, or backend server is required.

Do not add `server.js`, `package.json`, an `api/` folder, or a `vercel.json` from an older version to this static deployment. They are intentionally absent to prevent Vercel from trying to invoke a server function.

## Notes
- Chart.js and Google Fonts load from CDNs, so those visual enhancements need internet access.
- Data is saved in browser localStorage and does not automatically sync across devices.
- This is a personal finance dashboard, not a bank-connected application or financial advice service.

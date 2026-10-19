# Vercel deployment — static no-AI build

This package intentionally contains only static website assets. There is no Node server, API route, package.json, AI integration, or vercel.json.

1. Extract the ZIP.
2. Upload the files inside it directly to the repository root (not the ZIP itself and not an extra nested folder).
3. In Vercel, import the repository or redeploy the latest commit.
4. Set Framework Preset to **Other** and Root Directory to the repository root.
5. Keep Build Command and Output Directory overrides disabled/empty. No install command is needed.
6. Deploy and open the domain. Vercel should serve `index.html` as a static entry point.

If the old error persists, open Vercel → Project → Settings → Build and Deployment and verify the project is importing the intended repository and root directory. Then open Deployments → latest deployment → Build Logs. If the error says `FUNCTION_INVOCATION_FAILED`, check whether the deployed commit still contains an old `server.js`, `api/` directory, or configuration from the previous version.

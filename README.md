# Auction Resale Proxy (Stub, CommonJS)

This build uses **CommonJS** (`module.exports`) to avoid ESM config issues on Vercel.
Place these files at the **repo root** so the `api/` folder is at the top level.

## Deploy
1) New GitHub repo → upload these files (keep `api/` at repo root).
2) Vercel → Add New → Project → Import from Git → Deploy.
3) Test an endpoint in your browser (replace <your-app>):
   https://<your-app>.vercel.app/api/ebay-sold?q=test&site=US

If you still see 404:
- Confirm that the deployed repo contains `/api/ebay-sold.js` at the **root**.
- In Vercel, open **Project → Settings → Functions** and confirm Node functions are enabled.
- Check **Deployments → View Function Logs** for errors.

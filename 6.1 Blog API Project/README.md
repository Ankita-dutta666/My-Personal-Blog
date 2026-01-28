# Ankita Dutta - Personal Blog

Simple Express blog (frontend + in-memory API).

## Run locally

1. Install dependencies:

```bash
npm install
```

2. Start backend API (port 4000):

```bash
npm run api
```

3. Start frontend (port 3000) in another terminal:

```bash
npm start
```

4. Open http://localhost:3000


## Deploy to Railway (quick)

1. Push your repo to GitHub (root contains `6.1 Blog API Project`).
2. Go to https://railway.app and connect GitHub.
3. Create a new project → Deploy from GitHub → select your repo and set Root Directory to `6.1 Blog API Project`.

Backend service:
- Build command: `npm install`
- Start command: `npm run api`

Frontend service:
- Build command: `npm install`
- Start command: `npm start`
- Add environment variable `API_URL` = `<backend public URL>`

4. Deploy backend first, copy its public URL, then set `API_URL` for frontend and deploy frontend.

## Notes
- `server.js` reads `process.env.API_URL || "http://localhost:4000"`.
- `package.json` specifies Node engine `18.x` for hosts.

If you want, I can commit and push these changes for you or guide you through the Git commands to push.

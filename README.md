

## Local development

`https://developers.cloudflare.com/pages/functions/local-development/`

- Install Wrangler
  - `https://developers.cloudflare.com/workers/wrangler/install-and-update/`
  - `npm install wrangler --save-dev`
- Ensure `wrangler.toml` is set from [article](https://developers.cloudflare.com/pages/functions/local-development/)
- ​​Run your Pages project locally
  - `pkill -9 workerd && pkill -9 node`
  - `npx wrangler pages dev -- npm run dev`




Database

```
npx wrangler d1 execute montague \
  --local --command "CREATE TABLE IF NOT EXISTS user_test ( user_id INTEGER PRIMARY KEY, email_address TEXT, created_at INTEGER, deleted INTEGER, settings TEXT);"

```
# Vite+ Monorepo Starter

The Express API lives in `apps/server`. Run `vp run server#dev` in a separate
terminal alongside `vp run dev` for the website. The API defaults to port 3000;
`GET /api/health` returns `{ "ok": true }`. During development, the website
proxies `/api` requests to the server. If you change the API's `PORT`, update the
website proxy target to match. Production hosting must route `/api` separately.

A starter for creating a Vite+ monorepo.

## Development

- Check everything is ready:

```bash
vp run ready
```

- Run the tests:

```bash
vp run -r test
```

- Build the monorepo:

```bash
vp run -r build
```

- Run the development server:

```bash
vp run dev
```

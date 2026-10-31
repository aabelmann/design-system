Generic design system used to quickly setup a new project

Keywords:
- Minimal setup needed to get started
- Modern CSS only
  - CSS Variables
  - Always use latest technology which is supported by baseline
  - Extenable / Overridable (layers?)

Technology
- Nuxt 4+
- Plain CSS

## Run with Docker

Docker Compose runs Nuxt and its npm dependencies in the `node:26` container. No host Node.js or npm installation is needed.

```sh
docker compose up
```

Open http://localhost:3000. The workspace is mounted for live reload, while `node_modules` stays in a Docker-managed volume. On startup, the container runs `npm ci` from `package-lock.json`, then `npm start`.

Run Biome checks with:

```sh
docker compose run --rm nuxt sh -c "npm ci && npm run check"
```

Format supported files with:

```sh
docker compose run --rm nuxt sh -c "npm ci && npm run format"
```

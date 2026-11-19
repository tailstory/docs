# docs

Tailstory's org docs, for [docs.tailstory.dev](https://docs.tailstory.dev): everything that is not a library. Each library publishes its own docs under `/{package}/` from its own repository. A [Nimbus](https://nimbus-docs.com) site served as static assets from a Cloudflare Worker.

Pages are `src/content/docs/**/*.mdx`. Writing rules are in [AGENTS.md](AGENTS.md).

```sh
npm ci
npm run dev        # local preview
npm run typecheck
npm run build
npm run lint:docs
```

Needs the Node version in `.nvmrc`. Merges to `main` deploy.

Prose is [CC0](LICENSE).

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

## License

Copyright 2026 Tailstory.

- Prose (`src/content/`) is [CC BY 4.0](LICENSE-CC-BY-4.0). Credit "Tailstory" and link to the page you used.
- Everything else, and code samples inside the prose, is [Apache 2.0](LICENSE).

The site scaffolding comes from [Nimbus](https://github.com/cloudflare/nimbus) (MIT, copyright Cloudflare, Inc.). The fonts in `src/pages/og/_fonts/` are Inter (SIL Open Font License 1.1).

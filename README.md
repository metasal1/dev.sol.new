# dev.sol.new

Workshop site for **Superstack** — "Idea to Launch on Solana." A 45-minute walkthrough of building, validating, designing, and shipping a full Solana product from the terminal using Superstack's curated AI skill library.

Live: **https://dev.sol.new**

## Contents

| File | Live URL | What it is |
| --- | --- | --- |
| `index.html` | https://dev.sol.new/ | Landing page / directory of materials |
| `slides.html` | https://dev.sol.new/slides | 20-slide presentation deck (arrow keys to navigate) |
| `tutorial.html` | https://dev.sol.new/tutorial | Step-by-step guide, prerequisites to mainnet deploy |
| `handout.html` | https://dev.sol.new/handout | Printable one-page reference card |
| `assets/` | — | Solana logomark, Powered by Solana badge, avatar |

## Design

- **Font:** JetBrains Mono throughout.
- **No emojis** — decorative icons use the Solana logomark (`assets/sol-mark.svg`); callouts use plain monospace markers.
- **Branding:** every page carries the official [Powered by Solana](https://solana-icons.vercel.app) badge and a footer linking [metasal.xyz](https://metasal.xyz).

## Hosting

Static site on **Cloudflare Pages** (project `solana-new`), served at the canonical domain **dev.sol.new**.

Deploy a new version:

```sh
wrangler pages deploy . --project-name solana-new --branch main --commit-dirty=true
```

Cloudflare applies clean URLs automatically, so `/slides.html` redirects to `/slides`.

## License

MIT

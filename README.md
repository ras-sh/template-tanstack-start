# @ras-sh/template-tanstack-start

A production-ready template for quickly scaffolding TanStack Start projects with best practices and modern tooling.

## Features

- **[TanStack Start](https://tanstack.com/start)** - Full-stack React framework with file-based routing
- **React 19** - Latest React with modern features
- **TypeScript** - Full type safety with `@ras-sh/typescript-config`
- **Tailwind CSS v4** - Utility-first CSS with Vite plugin
- **@ras-sh/ui** - Component library built on Radix UI
- **Biome** - Fast linting and formatting via `ultracite`
- **Cloudflare Workers** - Ready for deployment with Wrangler
- **Geist Fonts** - Variable fonts for modern typography
- **Vite + SWC** - Fast builds and HMR

## Quick Start

```bash
pnpm install
pnpm dev
```

## Scripts

| Command | Description |
|---------|-------------|
| `pnpm dev` | Start development server (port 3000) |
| `pnpm build` | Build for production |
| `pnpm preview` | Preview production build |
| `pnpm deploy` | Deploy to Cloudflare Workers |
| `pnpm cf-typegen` | Generate Cloudflare Workers types |
| `pnpm check-types` | Run TypeScript type checking |
| `pnpm check` | Run linter checks |
| `pnpm fix` | Auto-fix linting issues |

## Project Structure

```
.
├── src/
│   ├── routes/              # File-based routing
│   ├── components/          # Reusable components
│   ├── lib/                 # Utilities (SEO helper, etc.)
│   ├── styles/              # Global styles
│   └── router.tsx           # Router configuration
├── public/                  # Static assets
├── vite.config.ts           # Vite configuration
└── wrangler.jsonc           # Cloudflare Workers configuration
```

## Deployment

```bash
pnpm deploy
```

Configured for Cloudflare Workers with Node.js compatibility enabled.

## License

MIT License - see the [LICENSE](LICENSE) file for details.

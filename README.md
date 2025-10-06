# @ras-sh/template-tanstack-start

🚀 A production-ready template for quickly scaffolding TanStack Start projects with best practices and modern tooling.

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

## Customization

This template is configured with ras.sh defaults. To customize for your own project:

### Required Changes

1. **package.json** - Update project metadata:
   - `name` - Your package name
   - `description` - Your app description
   - `homepage` - Your website URL
   - `bugs.url` - Your repository issues URL
   - `bugs.email` - Your support email
   - `repository.url` - Your repository URL
   - `author` - Your name, email, and website

2. **src/lib/seo.ts:18-19** - Update social media handles:
   - `twitter:creator` - Your Twitter handle
   - `twitter:site` - Your site's Twitter handle

3. **src/routes/__root.tsx:20-23** - Update default meta tags:
   - `title` - Your site title
   - `description` - Your site description

4. **public/site.webmanifest:2-3** - Update PWA manifest:
   - `name` - Your app name
   - `short_name` - Your app short name

5. **wrangler.jsonc:3** - Update Cloudflare Workers name:
   - `name` - Your worker name

6. **src/routes/index.tsx** - Replace with your landing page content

### Optional Changes

- **public/** - Replace favicon and icons with your own branding
- **LICENSE** - Update license holder if needed

## Scripts

| Command | Description |
|---------|-------------|
| `pnpm dev` | Start development server (port 5173) |
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

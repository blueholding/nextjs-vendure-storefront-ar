# متجر باندا - Panda Store

Vendure Next.js storefront configured for **PandaStore** with Arabic RTL support and Cloudflare Pages deployment.

## Quick Start

```bash
npm install
npm run dev
```

Open http://localhost:3001

## Environment Variables

Copy `.env.example` to `.env.local` and fill in:

```env
VENDURE_SHOP_API_URL=https://bramjlive.com/shop-api
NEXT_PUBLIC_VENDURE_SHOP_API_URL=https://pandastore.bramjlive.com/
VENDURE_CHANNEL_TOKEN=__default_channel__
NEXT_PUBLIC_SITE_URL=https://pandastore.bramjlive.com
NEXT_PUBLIC_SITE_NAME=متجر باندا
REVALIDATION_SECRET=your-secret-here
```

## Deploy to Cloudflare Pages

### From Cloudflare Dashboard

1. Connect your GitHub repo
2. Set **Build command**: `npm run build:cf`
3. Set **Output directory**: `.open-next/assets`
4. Add environment variables (see above)
5. Add **Compatibility flag**: `nodejs_compat`
6. Set **Compatibility date**: `2024-09-23`

### Environment Variables on Cloudflare

| Variable | Value |
|---|---|
| `VENDURE_SHOP_API_URL` | `https://bramjlive.com/shop-api` |
| `NEXT_PUBLIC_VENDURE_SHOP_API_URL` | `https://pandastore.bramjlive.com/` |
| `VENDURE_CHANNEL_TOKEN` | `__default_channel__` |
| `NEXT_PUBLIC_SITE_URL` | `https://pandastore.bramjlive.com` |
| `NEXT_PUBLIC_SITE_NAME` | `متجر باندا` |
| `REVALIDATION_SECRET` | `your-secure-random-string` |

## Languages

| Code | Language | Direction |
|---|---|---|
| `ar` | العربية (default) | RTL ← |
| `en` | English | LTR → |
| `de` | Deutsch | LTR → |

## Vendure Backend

- **Shop API**: https://bramjlive.com/shop-api
- **Admin Panel**: https://pandastore.bramjlive.com/

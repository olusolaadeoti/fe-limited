# Financing Enterprise Limited

A redesigned business finance website for Financing Enterprise Limited. The responsive homepage presents smaller loans, asset finance, and growth finance, alongside the company story, its approach, and an enquiry form.

Built with React 19, TypeScript, TanStack Start, Vite, and CSS. Netlify hosts the application, optimizes photography through Image CDN, and stores enquiries through Netlify Forms.

## Local development

Install dependencies with `pnpm install`, then run `netlify dev --port 8889`. Netlify Forms processes submissions on deployed sites; local development does not confirm live enquiry delivery.

## Content and assets

The homepage lives in `src/components/MarketingPage.tsx`, global design in `src/styles.css`, and page metadata in `src/data/site.ts`. The supplied brand artwork and extracted mark live in `public/img/`. Forest photography is sourced from Unsplash and stored locally.

Enquiries are submitted to `/__forms.html`. Received submissions can be reviewed in Netlify Forms. Submission notifications can be configured separately in the project dashboard. The form includes spam protection, pending, success, and retry states. No live submissions were sent during implementation.

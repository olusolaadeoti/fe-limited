# Financing Enterprise Limited

A responsive marketing website using React 19, TypeScript, TanStack Start, and the Netlify Vite adapter.

## Architecture

- `src/routes/index.tsx` renders the homepage.
- `src/routes/__root.tsx` provides the document, metadata, and global CSS.
- `src/components/MarketingPage.tsx` contains sections, expandable service details, mobile navigation, and the enquiry form.
- `src/data/site.ts` contains brand metadata.
- `src/styles.css` defines the evergreen and pale sage visual system, responsive layouts, and reduced motion support.
- `public/img/` contains the supplied brand original, extracted transparent mark, and locally stored Unsplash forest photography.
- `public/__forms.html` registers the enquiry form for deploy-time detection.

## Conventions and decisions

Use semantic HTML, labelled controls, visible keyboard focus, and meaningful link destinations. Keep browser APIs in event handlers. Preserve the supplied logo and source-verified business details. Avoid unsupported finance guarantees, invented statistics, rates, or regulatory claims.

The site is a complete marketing experience without accounts or an application database. Netlify Forms persists enquiries. Keep the React fields and static registration synchronized: `form-name`, `name`, `email`, `service`, `message`, and `bot-field`. POST to the static form path rather than the SSR homepage. Reject HTTP failures and unchanged registration HTML; retain entered details when submission fails. Do not log personal information.

Use Netlify Image CDN for photography. The cropped header mark is derived from the supplied artwork; the accompanying brand name is accessible text.

Use `pnpm install` and `netlify dev --port 8889` for local work. Build validation is handled by the platform pipeline. Finance descriptions are editorial website content, not quotes or loan offers.

# Dream Machinery / ড্রিম মেশিনারি

A mobile-first Bengali agricultural machinery storefront built with React and Vite. Frontend only: no backend, admin panel, real authentication, payment processing, or order submission.

## Run

```sh
npm install
npm run dev
```

## Verify

```sh
npm run build
npm test
```

## Included

- Custom vector leaf-and-gear logo in `public/logo.svg`.
- Responsive product catalogue with Bengali categories, search and price sorting.
- Product detail dialogs, local cart, quantity controls, and removal.
- Demo cash-on-delivery checkout. Form data is not sent anywhere or saved.
- Local demo profile (name and phone only); not real authentication.
- Dummy WhatsApp actions with explanatory notices.
- Owner-supplied YouTube video embedded on demand, with a YouTube fallback link.
- Keyboard escape handling, dialog focus containment, reduced-motion support.

## Content notes

The supplied Google image endpoints could not be downloaded in this environment (TLS connection failure). The current imagery is AI-generated, clearly disclosed in the footer and product details. Replace `public/images/machine-0.webp` through `machine-3.webp` with approved product photography. Product descriptions are generic category-level descriptions, not verified model specifications. All prices are samples between BDT 30,000 and 50,000. Delivery/service copy is a proposed demo presentation; the delivery information dialog explains that no operational policies are confirmed.

`dream-cart` and `dream-account` use browser localStorage. The profile can be removed from the account dialog. No passwords or payment details are requested. Google Fonts and the on-demand YouTube player are third-party network resources; there is no application server.

The test suite uses JSDOM against the production bundle. It checks user flows, not browser layout. A real Chromium download was unavailable in this environment, so cross-browser visual verification remains recommended.

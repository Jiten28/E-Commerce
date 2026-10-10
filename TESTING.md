# Validation notes

## Automated browser checks

169 assertions passed using Chromium against a local HTTP server, with no JavaScript runtime errors or missing resources in the tested flows.

Covered:
- Home catalogue and cross-page search
- Combined category, price and size filters; sorting; reset
- Persistent saved products
- Required size selection and gallery switching
- Persistent, variant-aware cart, quantity limits, item removal and recalculation
- Sample delivery threshold and INR totals
- Demo checkout validation and confirmation; bag clearing
- Local profile creation, persistence and removal
- Contact form demonstration
- No-results and missing-product states
- Mobile navigation, filter drawer and Escape dismissal
- All seven pages at 1440, 900, 768, 390 and 320px: horizontal overflow, empty links, unlabelled form fields and broken images

Additional long-query checks passed at 320, 390 and 1440px. Static checks confirmed local asset references and accessible dialog names.

## Visual review

25 page/state screenshots were reviewed individually, covering the seven routes on desktop and mobile plus navigation, search, filters, populated/empty bags, profile, no-results, product error feedback, privacy and checkout states. The logo and final homepage preview were also inspected. Long-query wrapping was corrected during this review.

Below-the-fold lazy-loaded images were explicitly loaded in isolated preview fixtures. Those testing fixtures and sample browser data are not included in the deliverable.

## Contrast and accessibility

Primary blue on white: 6.70:1. Muted text on white: 5.39:1; on the soft surface: 4.93:1. Form control boundaries on white: 3.55:1. Visible focus indicators, minimum 44px action targets, semantic form labels, dialog names and reduced-motion support are included.

These checks are not a formal accessibility certification or a substitute for testing across real browsers and assistive technologies.

## Not tested / not implemented

No real backend, payment, inventory, authentication, email delivery or order fulfilment exists in this frontend project. Safari, Firefox and real-device testing remain recommended before a production launch.

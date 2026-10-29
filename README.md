# Awesome-Checkout-Platform

# Awesome-Checkout-Platform

**Top Checkout Platform (Opensource) 🌟 Star if you like it! 🌟**



**Curated List of SaaS Products & Open-Source GitHub Projects**

*Focused on Hosted Checkout Pages, Payment Orchestration, One-Click Flows & Composable Commerce Checkout*

**Last updated: October 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Checkout Platforms**. These tools enable merchants to accept payments with minimal engineering effort—from fully hosted checkout pages that handle PCI compliance and payment method rendering to self-hosted commerce frameworks where the checkout is code you own and modify without constraints.



**Examples** include Shopify Checkout, Stripe Checkout, Adyen Checkout, Checkout.com, PayPal Checkout, Klarna Checkout, Square Checkout, Amazon Pay, Bolt, and Fast (the category leaders and cautionary tales in commercial space).



**Open-source emphasis**: This section is expanded with every relevant project for self-hosting, checkout flows, and open payment infrastructure. **Critical note**: True open-source checkout platforms—hosted pages with PCI-compliant card forms and built-in payment method support—do not exist as turnkey SaaS replacements. Open-source projects provide **commerce frameworks** where you build and host the checkout yourself, or **payment orchestration layers** that route transactions but do not render a checkout UI. The projects below require you to own the infrastructure, PCI compliance, and payment processor relationships.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[Shopify Checkout](https://www.shopify.com/)**

  **Fully hosted, PCI-compliant checkout** with Shop Pay acceleration, dynamic upsells, and extensive payment method support. Checkout is highly customizable via Shopify Functions and Checkout UI Extensions, but the core flow is hosted by Shopify and not self-hostable. **Pricing**: Included with Shopify plans (from $39/month Basic to $399/month Plus). **Free tier**: None. **Best for**: merchants wanting a managed checkout with the largest accelerated wallet network (Shop Pay) and no PCI burden.



- **[Stripe Checkout](https://stripe.com/payments/checkout)**

  **Hosted checkout page** that handles card entry, wallets, and localized payment methods with a single API call. Supports subscriptions, trials, and tax calculation. **Pricing**: Standard Stripe processing fees (2.9% + $0.30 for cards). **Free tier**: None for payments. **Best for**: developers wanting the fastest integration path to a PCI-compliant, conversion-optimized checkout with minimal code.



- **[Adyen Checkout](https://www.adyen.com/)**

  **Enterprise checkout and payment processing** with a unified API across channels (online, in-person, mobile). **Pricing**: Quote-only; interchange-plus or blended models. **Free tier**: None. **Best for**: enterprises wanting a single platform for online and offline payments with global payment method coverage.



- **[Checkout.com](https://www.checkout.com/)**

  **Enterprise payment processing** with hosted checkout, tokens, and fraud tools. **Pricing**: Quote-only; interchange-plus models. **Free tier**: None. **Best for**: large merchants wanting a modern processor with direct acquiring relationships and strong API tooling.



- **[PayPal Checkout](https://www.paypal.com/)**

  **Hosted checkout experience** with PayPal, Venmo, Pay Later, and card processing. Includes Smart Payment Buttons that dynamically present relevant options. **Pricing**: Standard PayPal merchant fees. **Free tier**: None. **Best for**: merchants wanting access to PayPal's 400M+ active accounts and buyer protection without building wallet integrations.



- **[Klarna Checkout](https://www.klarna.com/)**

  **BNPL-native checkout** that integrates Pay in 4, Pay in 30 days, and financing options directly into the checkout flow. **Pricing**: Merchant fees per transaction. **Free tier**: None. **Best for**: merchants targeting BNPL-preferring demographics wanting installment options embedded in checkout.



- **[Square Checkout](https://squareup.com/)**

  **Hosted checkout and payment links** integrated with Square's POS and online ecosystem. **Pricing**: 2.9% + $0.30 per online transaction. **Free tier**: None for payments. **Best for**: omnichannel merchants already using Square for in-person payments wanting unified online checkout.



- **[Amazon Pay](https://pay.amazon.com/)**

  **Amazon account-based checkout** using saved addresses and payment methods. **Pricing**: Standard Amazon Pay merchant fees. **Free tier**: None. **Best for**: merchants selling to Amazon-accustomed shoppers wanting a trusted, recognizable checkout option.



- **[Bolt](https://www.bolt.com/)**

  **One-click checkout and identity platform** offering hosted, embeddable, and buy-now links. **Valuation collapsed 97%** from $11B to $300M; currently raising a **$27M pay-to-play bridge round** with CEO personally committing $5M; headcount reduced from 900 to ~60. **Pricing**: Quote-only. **Free tier**: None. **Best for**: merchants evaluating alternatives to Shop Pay with full awareness of vendor stability risk.



- **[Fast](https://fast.co/)** (**Defunct**)

  **One-click checkout startup that shut down abruptly in April 2022** after raising ~$125M and burning ~$10M/month on just $600K in annual revenue. Widely cited as a cautionary tale about competing against entrenched wallet networks without sustainable unit economics. **Pricing**: N/A. **Free tier**: N/A. **Best for**: historical reference only—**do not build on this platform**.



## Open-Source GitHub Projects



- **[Spree Storefront](https://github.com/spree/storefront)**

  **Open-source Next.js storefront with one-page checkout** (MIT) — **the most production-ready open-source checkout UI** in this list. **Features**: One-page checkout supporting guest and authenticated users; multi-shipment natively; coupon codes, gift cards, and store credit; **Stripe, PayPal, and Adyen via Payment Sessions** with 3DS, Apple Pay, Google Pay, Klarna, Affirm, and SEPA support; card data never touches your server; transactional emails via Resend; multi-region with country/currency/language switching . **Tech stack**: Next.js 16, React 19, TypeScript, Tailwind CSS 4. **Deploy**: Self-hosted (point `NEXT_PUBLIC_SPREE_API_URL` at a Spree backend). **Trade-off**: **Storefront UI only**—requires a Spree Commerce backend (BSD-3-Clause) running separately. You own PCI compliance and payment processor relationships. **Best for**: developers wanting a production-ready, customizable one-page checkout with swappable payment providers and no SaaS lock-in.



- **[Medusa](https://github.com/medusajs/medusa)**

  **Open-source headless commerce platform** (MIT for core) — **a composable framework where checkout is fully yours to build and host**. **Features**: Modular architecture with separate cart, payment, and fulfillment modules; API-first; the payment step flow includes retrieving providers, creating payment collections, and initializing payment sessions via SDK . **Tech stack**: Node.js, TypeScript, PostgreSQL. **Deploy**: Self-hosted or Medusa Cloud. **Trade-off**: **Not a checkout platform out of the box**—you build the checkout UI and flow in your storefront. No pre-built hosted checkout page. **Best for**: developers wanting full ownership of checkout logic within a modern TypeScript stack.



- **[Saleor](https://github.com/saleor/saleor)**

  **Open-source, GraphQL-first headless commerce platform** (BSD-3-Clause) — **a mature composable framework with a rich checkout API**. **Features**: Single GraphQL endpoint covering checkout, orders, payments, and promotions; official TypeScript/JavaScript SDK with typed checkout helpers; reference Next.js storefront for checkout flows . **Tech stack**: Python (Django), GraphQL, PostgreSQL. **Deploy**: Self-hosted or Saleor Cloud. **Trade-off**: **Platform, not a hosted checkout**—checkout must be implemented in a storefront using the GraphQL API. No built-in UI. **Best for**: teams wanting a GraphQL-native commerce backend with fine-grained control over checkout mutations and pricing.



- **[Vendure](https://github.com/vendure-ecommerce/vendure)**

  **Open-source headless commerce framework** (MIT) — **a TypeScript-first platform with an official storefront starter that includes checkout**. **Features**: The **TanStack Start Storefront Starter** covers cart management, promotion codes, shipping selection, payment, checkout review, and order confirmation; English and German localization; persistent currency selection . **Tech stack**: Node.js, TypeScript, GraphQL, PostgreSQL. **Deploy**: Self-hosted (clone starter, point at Vendure Shop API). **Trade-off**: **Framework + starter**—checkout is code you own and modify; no hosted checkout page. **Best for**: TypeScript developers wanting a modern commerce framework with an official storefront that includes a complete checkout flow.



- **[Sylius](https://github.com/Sylius/Sylius)**

  **Open-source eCommerce framework for Symfony** (MIT) — **a PHP-based framework with complete control over checkout flow**. **Features**: Custom checkout flows, tiered pricing, organization-level accounts, and tax logic built to match your business; headless and API-first, pairable with any frontend; Community Edition is MIT-licensed . **Tech stack**: PHP (Symfony), Doctrine. **Deploy**: Self-hosted. **Trade-off**: **Framework, not a checkout platform**—you build and host the checkout within your Symfony application. No pre-built UI or hosted page. **Best for**: PHP/Symfony developers wanting full control over checkout logic in a mature, MIT-licensed framework.



- **[Hyperswitch](https://github.com/juspay/hyperswitch)**

  **Open-source payment orchestration platform** (Apache 2.0 for core) — **the most significant open-source infrastructure for the payment layer beneath checkout**. **Features**: Unified orchestration across 100+ processors and networks; dynamic routing and smart retries to improve authorization rates; vault, reconciliation, cost observability, and APM widgets; composable modules you can adopt independently . **Tech stack**: Rust (backend), TypeScript/React. **Deploy**: Self-hosted (Docker, Kubernetes) or Hyperswitch Cloud. **Trade-off**: **Orchestration layer, not a checkout UI**—it routes transactions and manages payment methods but does not render a checkout page. You still build the frontend. **Best for**: merchants wanting to reduce processor lock-in, improve success rates via routing, and own their payment infrastructure without building orchestration from scratch.



- **[Liberu Ecommerce](https://github.com/liberusoftware/ecommerce-laravel)**

  **Open-source Laravel eCommerce platform** (MIT) — **a full-stack option with reactive checkout built in**. **Features**: Reactive shopping cart and checkout with Livewire 4; guest and authenticated checkout flows; multiple shipping methods with server-side rate calculation; Stripe integration with webhooks and test mode; PayPal ready to activate; dropshipping via DropXL . **Tech stack**: Laravel 13, PHP 8.5, Filament 5, Livewire 4. **Deploy**: Self-hosted (`./setup.sh` interactive installer). **Trade-off**: **Full platform, not a checkout component**—you adopt the entire ecommerce stack. No hosted checkout; PCI compliance is your responsibility. **Best for**: Laravel developers wanting a modern, full-stack commerce platform with checkout included.



### Additional Strong Open-Source Options



- **Mobazha Unified** — Open-source commerce frontend for storefronts, marketplaces, and checkout (MPL-2.0). Connects to hosted or self-hosted Mobazha Node; renders payment networks advertised by backend (UTXO chains, EVM networks including BNB Smart Chain); per-order Safe multisig escrow addresses . **Note**: Crypto-native checkout focus—not traditional card processing. **Best for**: merchants in crypto commerce wanting a self-hostable checkout frontend.

- **Spwig Commerce** — Modular monolith Django eCommerce platform (AGPL-3.0). Includes storefront, admin, REST API, and Celery workers in a single process; provider SDKs for payments are Apache-2.0 . **Note**: Full platform, not a checkout component; requires adopting the entire stack. **Best for**: Django developers wanting a batteries-included commerce platform.



**Frameworks for building custom systems**: Combine **Spree Storefront** for a production-ready one-page checkout UI with **Spree Commerce** or **Medusa** as the backend, **Hyperswitch** for payment orchestration and routing, and **Vendure** or **Saleor** for GraphQL-native commerce—creating a self-hosted checkout stack. **None of these provide a hosted, PCI-compliant checkout page** like Stripe Checkout or Shopify Checkout; you own the infrastructure, compliance, and processor relationships.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, license (for open-source), and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Checkout platforms handling payment data must comply with **PCI DSS**, data protection regulations (GDPR, CCPA, etc.), and card network rules. Self-hosted solutions shift PCI compliance responsibility to you.

- **The "hosted checkout page" vs. "commerce framework" vs. "payment orchestration" distinction is absolute.** **Shopify Checkout, Stripe Checkout, Adyen Checkout, Checkout.com, PayPal Checkout, Klarna Checkout, Square Checkout, Amazon Pay, and Bolt** are **hosted checkout services**—they render the payment UI, handle PCI compliance, and often provide optimized conversion flows. **Spree Storefront, Medusa, Saleor, Vendure, Sylius, and Liberu** are **commerce frameworks**—they provide the backend and/or storefront code, but **you host the checkout and own PCI compliance**. **Hyperswitch** is **payment orchestration**—it routes transactions but does not render a checkout page. **No open-source project provides a turnkey hosted checkout SaaS replacement.**

- **Fast is included as a historical cautionary tale, not a recommendation.** The company shut down in April 2022 after raising ~$125M and burning ~$10M/month on ~$600K annual revenue. Its failure illustrates the difficulty of competing against entrenched payment networks without sustainable economics. **Do not build on defunct infrastructure.**

- **Bolt's stability is uncertain.** Its valuation collapsed 97% from $11B to $300M, and it is raising a pay-to-play bridge round described as potentially the company's last shot. **Evaluate vendor risk carefully before committing.**

- **Spree Storefront is the strongest open-source checkout UI in this list.** It offers a production-ready one-page checkout with Stripe, PayPal, and Adyen, wallet support (Apple Pay, Google Pay, Klarna, Affirm), and multi-region capabilities . **The trade-off**: it requires a Spree Commerce backend and shifts PCI compliance to you.

- **Open-source checkout requires accepting PCI responsibility.** When you self-host a checkout, you are handling card data (or integrating a processor's iframe/SDK). **This is a significant operational and compliance burden** that hosted checkouts like Stripe eliminate. Evaluate your team's capacity for PCI DSS compliance before choosing an open-source path.

- **Pricing opacity varies.** Stripe Checkout and Square publish standard processing rates; Shopify includes checkout with platform subscriptions. Adyen, Checkout.com, PayPal (enterprise), Klarna, Amazon Pay, and Bolt require sales contact or volume-based negotiation. **Validate with direct vendor conversations against your transaction volume and payment mix.**

- Self-hosted open-source solutions require proper server setup, security hardening, backup configuration, and ongoing maintenance. **Checkout code handles payment credentials**—ensure your deployment meets PCI DSS requirements and your organization's security standards before processing live transactions.



---



**Made for developers, merchants, and organizations building transparent checkout infrastructure.**

Let's make Checkout Platforms more open, data-driven, and merchant-friendly.

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

- [Sector Overview & Market Dynamics](#sector-overview--market-dynamics)
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## Sector Overview & Market Dynamics

The global payment gateway and checkout platform market is estimated at **$35B – $58B in 2026** and projected to surpass **$240B+ by the mid-2030s** (growing at an estimated 14%–22% CAGR). The sector is **moderately fragmented yet increasingly concentrated around dominant ecosystem winners**—where top players like Amazon, Shopify, Stripe, PayPal, and Adyen capture massive transaction volumes, while specialized and independent one-click checkout providers face steep network-effect barriers and margin pressure.

## SaaS/Hosted Platforms

| Platform | Company Size (Valuation / Revenue) | Starting Pricing Tier | Free Tier Limits / Free Trial | Best For & Overview |
| :--- | :--- | :--- | :--- | :--- |
| **[Amazon Pay](https://pay.amazon.com/)** | **~$2.68T Market Cap** (~$716.9B annual revenue) | 2.9% + $0.30 per domestic web/mobile transaction ($0 setup/monthly fees) | **No Free Trial**: Unlimited sandbox test environment included; live processing has no free transaction tier (fees apply on successful live transactions). | Merchants seeking trusted 1-click checkout leveraging Amazon accounts and buyer credentials. |
| **[Shopify Checkout](https://www.shopify.com/)** | **~$220B Market Cap** (~$8.9B annual revenue) | Basic plan starting at **$39/month** (+ 2.9% + $0.30 per online transaction with Shopify Payments) | **3-Day Free Trial** (then $1/month promo for 3 months): Unlimited store build/admin testing; live checkout is locked in password-protected mode until a paid plan is selected. | Merchants wanting a turn-key managed checkout with the Shop Pay network without PCI burdens. |
| **[Stripe Checkout](https://stripe.com/payments/checkout)** | **~$159B Private Valuation** (~$4.2B+ net revenue) | **2.9% + $0.30** per successful card charge (Pay-as-you-go, no monthly fee) | **No Live Free Tier**: Free perpetual Sandbox/Test Mode (full API & UI simulator, up to 730-day trial simulation); live mode has no free transaction allotment. | Developers wanting the fastest integration to a conversion-optimized, PCI-compliant hosted checkout. |
| **[PayPal Checkout](https://www.paypal.com/)** | **~$46B Market Cap** (~$31.8B annual revenue) | **3.49% + $0.49** per PayPal/Venmo checkout transaction (**2.99% + $0.49** for standard card processing) | **No Free Tier**: Free perpetual developer sandbox access; live checkout charges per processed order with zero free allowance. | Merchants looking for immediate access to 400M+ active PayPal and Venmo wallet users. |
| **[Square Checkout](https://squareup.com/)** | **~$45B Market Cap** (Parent Block; ~$24.1B annual revenue) | **$0/month** software fee with **3.3% + $0.30** per online transaction (or **2.9% + $0.30** via Square Online APIs / $49/mo Plus plan) | **Free-Forever Plan**: Unlimited products, full POS sync, and online payment links; limited to basic store templates, standard reporting, and 3.3% + 30¢ processing rate. | Omnichannel merchants unifying online checkout and in-person POS sales with zero upfront monthly cost. |
| **[Adyen Checkout](https://www.adyen.com/)** | **~$30B Market Cap** (~€1.9B net revenue) | Interchange++ starting from **$0.12 fixed fee + 0.40%–0.60% markup** per transaction (typically €100–€500/mo minimum volume) | **No Free Tier**: Free test/sandbox environment for enterprise integration; live processing requires approved commercial contract with monthly minimums. | Global enterprises requiring unified cross-channel online/in-store processing and international acquiring. |
| **[Checkout.com](https://www.checkout.com/)** | **~$12B Valuation** (~$500M+ revenue) | Interchange++ custom quote (starting base markup of **~0.25%–0.50% + $0.05–$0.10** per transaction with zero monthly gateway fee) | **No Free Tier**: Dedicated sandbox testing environment; live transactions require merchant underwriting and commercial contract. | High-volume merchants and modern fintechs requiring direct acquiring relationships and granular payment APIs. |
| **[Klarna Checkout](https://www.klarna.com/)** | **~$4.8B Valuation / Market Cap** (~$2.8B revenue) | **5.99% + $0.30** per transaction for standard BNPL (or ~2.99% + $0.30 for Pay Now; scales to 3.29% + $0.30 for high volume) | **No Free Tier**: Playground/test credentials available for integration; zero free transactions on live production orders. | Merchants targeting younger demographics seeking seamless embedded Buy Now Pay Later (Pay in 4 / 30). |
| **[Bolt](https://www.bolt.com/)** | **~$300M Valuation** (down from $11B peak; ~$30M revenue) | Baseline starting rate of **2.9% + $0.30** per transaction or custom markup over existing processor gateway | **No Free Tier**: Sandbox developer portal for testing; live deployment requires enterprise agreement. | Merchants exploring standalone alternative 1-click networks aware of ongoing platform volatility. |
| **[Fast](https://fast.co/)** | **$0 / Defunct** (Shut down April 2022 after raising $125M; peaked at $600K ARR) | Defunct (**N/A**; previously charged ~2.9% + $0.30) | **Defunct**: Zero active tiers or trials. Retained as historical case study on unsustainable wallet subsidies. | Historical reference only; do not build on this platform. |

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

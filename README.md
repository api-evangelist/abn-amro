# ABN AMRO (abn-amro)
A Dutch banking and financial services group serving retail, private, and corporate clients across Europe. ABN AMRO publishes a public developer portal exposing PSD2 Open Banking, Tikkie payment-request, and corporate payment APIs.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/abn-amro/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=abn-amro-api-evangelist&utm_content=repo)

## Tags:

 - Financial, Banks, European Banking, Open Banking, PSD2, Payments

## Timestamps

- **Created:** 2026-05-05
- **Modified:** 2026-05-16

## APIs

### Tikkie API
The Tikkie API lets Tikkie Business customers programmatically create payment requests, send them to end-payers, and receive notifications when payments complete.

**Human URL:** [https://developer.abnamro.com/api-products/tikkie/overview](https://developer.abnamro.com/api-products/tikkie/overview)

#### Tags:

 - Payments, Payment Requests, Consumer Finance

#### Properties

- [Documentation](https://developer.abnamro.com/api-products/tikkie/overview)
- [ReferenceDocumentation](https://developer.abnamro.com/api-products/tikkie/reference-documentation)

### Payment Initiation (PSD2) API
PSD2-compliant Payment Initiation Service allowing licensed Third Party Providers (TPPs) to initiate SEPA payments from ABN AMRO accounts. Requires a PSD2 eIDAS certificate.

**Human URL:** [https://developer.abnamro.com/api-products/payment-initiation-psd2/overview](https://developer.abnamro.com/api-products/payment-initiation-psd2/overview)

#### Tags:

 - Open Banking, PSD2, Payments, Payment Initiation

#### Properties

- [Documentation](https://developer.abnamro.com/api-products/payment-initiation-psd2/overview)
- [ReferenceDocumentation](https://developer.abnamro.com/api-products/payment-initiation-psd2/reference-documentation)

### Business Account Payment API
Corporate / business-account payment API for ABN AMRO commercial customers to initiate payments and retrieve transaction status. Uses OAuth 2.0 client-credentials with mTLS.

**Human URL:** [https://developer.abnamro.com/api-products/business-account-payment/overview](https://developer.abnamro.com/api-products/business-account-payment/overview)

#### Tags:

 - Payments, Corporate Banking, SEPA

#### Properties

- [Documentation](https://developer.abnamro.com/api-products/business-account-payment/overview)
- [ReferenceDocumentation](https://developer.abnamro.com/api-products/business-account-payment/reference-documentation)

## Common Properties

- [Website](https://www.abnamro.com/)
- [Portal](https://developer.abnamro.com/)
- [Documentation](https://developer.abnamro.com/)
- [GettingStarted](https://developer.abnamro.com/get-started)
- [TermsOfService](https://developer.abnamro.com/content/terms-and-conditions)

## Features

| Name | Description |
|------|-------------|
| Payment Requests | Create Tikkie payment requests and receive callbacks when an end-payer settles them. |
| PSD2 Payment Initiation | Initiate SEPA Credit Transfer and SEPA Instant payments under PSD2 PIS for both retail and business accounts. |
| Corporate Payments | Submit own-account corporate payments and retrieve detailed transaction status. |
| OAuth 2.0 Authorization | Authorization Code (with PKCE) and Client Credentials flows for licensed TPPs and direct business clients. |
| eIDAS Certificate Onboarding | PSD2 production access uses qualified eIDAS certificates (QWAC + QSeal) for transport and signing. |
| Sandbox | Public sandbox with test certificates and synthetic accounts for all PSD2 and business-payment APIs. |

## Use Cases

| Name | Description |
|------|-------------|
| Merchant Payment Collection | Use Tikkie to send a one-off or recurring payment request to a customer over a link instead of card-present checkout. |
| Account-to-Account Checkout | Use PSD2 Payment Initiation as a low-cost alternative to card rails for e-commerce checkout in the Netherlands and EU. |
| Corporate Treasury Automation | Automate payroll, supplier payments, and treasury transfers from ABN AMRO business accounts. |
| TPP Aggregation | PSD2 TPPs (PISP role) routing customer-authorized payments through ABN AMRO as one of the Dutch banks they cover. |

## Authentication

| Name | Description |
|------|-------------|
| API Token (Tikkie) | Server-side API token issued via the Tikkie Business portal for Tikkie-only calls. |
| OAuth 2.0 Authorization Code | Three-legged OAuth 2.0 with PKCE for PSD2 user-consent flows. |
| OAuth 2.0 Client Credentials + mTLS | Two-legged OAuth 2.0 with mutual TLS using eIDAS QWAC for PSD2 and business-account APIs. |
| eIDAS Qualified Certificates | PSD2 production access requires QWAC for transport and QSeal for request signing per Berlin Group NextGenPSD2. |

## Compliance

| Name | Description |
|------|-------------|
| PSD2 | Revised Payment Services Directive (EU 2015/2366) — ABN AMRO is a regulated ASPSP exposing PIS and AIS endpoints. |
| Berlin Group NextGenPSD2 | ABN AMRO follows the Berlin Group NextGenPSD2 XS2A framework for its PSD2 APIs. |
| GDPR | General Data Protection Regulation compliance for personal data processed by the APIs. |
| DNB / ECB Supervision | Supervised by De Nederlandsche Bank (DNB) and indirectly by the European Central Bank as a significant institution. |
| ISO 20022 | SEPA payment payloads align with ISO 20022 pain.* and camt.* messages where applicable. |

## Integrations

| Name | Description |
|------|-------------|
| Tikkie | ABN AMRO subsidiary providing the Tikkie consumer and business payment-request product. |
| Berlin Group XS2A | Common European PSD2 specification used by ABN AMRO and most Dutch and German banks. |
| Open Banking Aggregators | PSD2 aggregators (e.g., Tink, TrueLayer, Plaid Europe) connect to ABN AMRO via the PSD2 endpoints. |

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com

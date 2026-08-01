# Somatus

Somatus is a value-based kidney and heart care management company founded in 2016 and headquartered in
McLean, Virginia. It partners with health plans, provider groups and nephrology practices to slow the
progression of chronic kidney disease (CKD), end-stage kidney disease (ESKD) and congestive heart failure,
surrounding patients with in-home and virtual care teams of nurses, community health workers, pharmacists,
dietitians and social workers across all 50 states and DC.

Its proprietary **RenalIQ** technology platform applies predictive analytics and machine learning across
claims, clinical and social data to prioritize care-team interventions, and is surfaced to partners through
a patient portal (`my.somatus.com`) and a provider / health-plan self-service portal (`connect.renaliq.com`).

- Website: https://somatus.com/
- Technology: https://somatus.com/how-it-works/our-technology/
- Providers: https://somatus.com/providers/ · Health Plans: https://somatus.com/health-plans/
- Provider portal: https://connect.renaliq.com/ · Patient portal: https://my.somatus.com/

## API surface

**Somatus publishes no public API.** As of the 2026-07-31 enrichment pass there is no developer portal, no
API documentation, no machine-readable contract, and no first-party SDK or CLI. Contract discovery probed
`somatus.com`, `my.somatus.com` and `connect.renaliq.com` for `/openapi.json`, `/openapi.yaml`,
`/swagger.json`, `/api-docs`, `/docs`, `/graphql`, and the full `/.well-known/` discovery surface — every
path 404s (`my.somatus.com` is a single-page-app catch-all that answers 200 with an HTML shell for every
path; those are not documents). npm, PyPI and the candidate GitHub organizations carry no published
Somatus packages or public repositories. RenalIQ is delivered as a partner portal, not an API product.

## What this repo does capture

| Artifact | File | Method |
|---|---|---|
| llms.txt | `llms/somatus-llms.txt` | searched — published verbatim at `somatus.com/llms.txt` |
| Well-known probe index | `well-known/somatus-well-known.yml` | probed |
| Conformance / accreditations | `conformance/somatus-conformance.yml` | searched |
| Domain security | `security/somatus-domain-security.yml` | probed |

## Compliance posture

HITRUST CSF r2 Certified (RENALIQ platform), NCQA Accredited for Case Management, Population Health
Program, and Health Equity — the first and only value-based kidney care management provider with the NCQA
Health Equity accreditation. Signed the Health Evolution Forum Health Equity Pledge in October 2023.

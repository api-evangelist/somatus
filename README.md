# Somatus

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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

# Ebix (ebix)

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
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Ebix is a United States insurance software and exchange company headquartered in Johns Creek, Georgia, operating as market infrastructure between carriers, MGAs, brokers and agencies rather than as a carrier itself. Its portfolio spans property and casualty agency management (EbixASP), P&C policy administration and placing (EbixEvolution, PlacingHub, Sunrise Exchange, iClose), life and annuity distribution connectivity (EbixExchange), health insurance and employee benefits administration, health content, risk and compliance (RiskEnvision, WCExchange), and — through the EbixCash arm — travel, payments and forex services.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/ebix/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/ebix/refs/heads/main/apis.yml)

## Tags

- Insurance
- United States
- Property and Casualty
- Life Insurance
- Health Insurance
- Employee Benefits
- Agency Management
- Policy Administration
- Claims
- ACORD
- Insurtech
- Market Infrastructure

## Timestamps

- **Created:** 2026-07-25
- **Modified:** 2026-07-25

## APIs

None listed. Ebix publishes **no public, self-serve developer portal and no retrievable machine-readable API specification** as of 2026-07-25.

This is the expected shape for United States insurance infrastructure: there is no federal insurance regulator and no open-insurance mandate, so nothing forces a public API surface, and integration is sold and documented under contract.

### What was actually probed

| Surface | Status | Finding |
| --- | --- | --- |
| `https://www.ebix.com/developers` | 200 | Soft 404 — serves the identical homepage SPA shell |
| `https://www.ebix.com/developer` | 200 | Soft 404 — identical homepage SPA shell |
| `https://www.ebix.com/api` | 200 | Soft 404 — identical homepage SPA shell |
| `https://www.ebix.com/partners` | 200 | Soft 404 — identical homepage SPA shell |
| `https://www.ebix.com/integrations` | 200 | Soft 404 — identical homepage SPA shell |
| `https://developer.ebix.com` | — | DNS does not resolve |
| `https://docs.ebix.com` | — | DNS does not resolve |
| `https://developers.ebix.com` | — | Connection timed out |
| `https://api.ebix.com/` | 404 | Live gateway, `{ "statusCode": 404, "message": "Resource not found" }`, no public routes |
| `https://api.ebixcash.com/` | 200 | Live "Ebixcash API Hub" (uvicorn/FastAPI) |
| `https://api.ebixcash.com/openapi.json` | **401** | The OpenAPI document exists but is gated: `{"detail":"Missing Authorization header"}` |
| `https://www.ebixasp.com/api` | 404 | IIS 404 |

No OpenAPI, Swagger, AsyncAPI, GraphQL SDL, `.proto`, webhook catalog or official Postman workspace could be retrieved anonymously. Nothing was fabricated to fill the gap, so there is no `openapi/` directory in this repo.

## Artifacts

Enrichment round 2026-07-25 re-probed every host and captured what is genuinely published:

| Artifact | Method | Result |
| --- | --- | --- |
| [`llms/ebix-llms.txt`](llms/ebix-llms.txt) | **searched** | **Real `llms.txt` found and saved verbatim** — `https://www.ebix.com/llms.txt` returns 6,650 bytes of markdown (generated with the LLMs.txt Generator Tool) indexing the solution, service, news and legal pages. It names no API, no portal and no specification. |
| [`well-known/ebix-well-known.yml`](well-known/ebix-well-known.yml) | probed | Zero real `/.well-known/` documents on any host. `www.ebix.com` answers **200 with the homepage shell for every path**, so its `/.well-known/security.txt` and `/.well-known/openid-configuration` "200"s are soft 404s, recorded as such. No `WellKnown`/`SecurityTxt` pointer is wired. |
| [`conformance/ebix-conformance.yml`](conformance/ebix-conformance.yml) | searched | The conforming standards are **insurance data standards, not web-API standards**: ACORD AL3, ACORD AL3 Claims Download, ACORD XML, the ACORD forms library, the IVANS real-time interface, plus `llms.txt`. OpenAPI is `unknown` (exists but 401-gated); AsyncAPI, GraphQL, gRPC, OIDC, RFC 9457, RFC 9116 and RFC 8594 are all `false`. No ACORD certification and no NGDS reference is published. |
| [`authentication/ebix-authentication.yml`](authentication/ebix-authentication.yml) | probed | `documented: false`. Records the wire evidence only — the undisclosed `Authorization` requirement on the EbixCash API Hub, the EbixASP `/support` form login, and IVANS-provisioned carrier credentials. No `Authentication` pointer is wired, because nothing is documented. |
| [`security/ebix-domain-security.yml`](security/ebix-domain-security.yml) | probed | `www.ebix.com` TLSv1.2, HSTS `max-age=31536000`, cert to 2026-11-25; `ebix.com` has SPF and DMARC at `p=quarantine`, **no DNSSEC and no CAA**. |
| Packages / SDKs | searched | **None.** npm, PyPI, RubyGems, NuGet, Packagist, crates.io and Maven Central return no first-party Ebix client library (`ebixui` on npm is an unrelated Vue component library). No `packages/` or `SDKs` pointer. |
| Vulnerability disclosure / trust center | probed | **None.** `trust.ebix.com` does not resolve; `/security` and `/compliance` are SPA soft 404s; no bug-bounty program and no named certification (SOC 2, ISO 27001, PCI DSS, HIPAA, FedRAMP) is published. No `Security`, `Compliance` or `TrustCenter` pointer. |
| Status page | probed | **None.** `ebix.statuspage.io` resolves but reads *"Ebix Status — Page Inactive"*; `status.ebix.com` does not resolve. No `StatusPage` pointer. |
| GitHub | searched | No first-party org. `github.com/Ebix-Inc` exists as an empty organization (0 public repos, no profile metadata tying it to ebix.com) and `github.com/ebix` is an unrelated 2011 user account. No `GitHubOrganization` pointer. |
| MCP / skills / Arazzo / overlays / errors / scopes / data model | — | Not applicable: all of these derive from an OpenAPI, and no spec could be retrieved. Nothing was generated. |

## ACORD posture

**ACORD AL3 + ACORD XML download/upload translation, delivered with the IVANS real-time interface.**

Ebix's P&C plumbing is ACORD-native rather than API-native, and the evidence is explicit and first-party:

- *"TEAM-UP uses ACORD-standard AL3 files, ensuring universal acceptance across all agency management systems that support the standard."* — [TEAM-UP](https://www.ebix.com/solutions/property-and-casualty-insurance/team-up)
- *"In addition to policy downloads, TEAM-UP supports Claims Download and Direct Bill Commission Download."* — [TEAM-UP](https://www.ebix.com/solutions/property-and-casualty-insurance/team-up)
- *"Ebix has extensive experience translating carrier-specific formats into ACORD AL3."* — [Translation Services](https://www.ebix.com/solutions/property-and-casualty-insurance/translation-services)
- *"Ebix maintains pre-built ACORD templates for each line of business, along with established data definitions, schemas, and mappings for nearly all supported download LOBs."* — [Translation Services](https://www.ebix.com/solutions/property-and-casualty-insurance/translation-services)
- *"EbixASP utilizes a library of ACORD forms that is updated constantly … EbixASP utilizes bi-directional data exchange with ACORD applications."* — [EbixASP brochure](https://www.ebix.com/pdf/asp_web.pdf)
- *"EbixeForms uses electronic ACORD Forms for entry of data by an Agent/Broker for submission to Carriers and MGAs. XML Data is separated from the electronic form…"* — [EbixeForms brochure](https://www.ebix.com/pdf/eforms_web.pdf)
- *"When logging onto the EbixASP Real Time Interface the PC synchronizes with IVANS and updates the credentials on the PC…"* — [EbixASP help](https://www.ebixasp.com/ebixasphelp/maintenance/Real_Time_Interface/Install_Download_Real-Time_Interface.htm)

No NGDS reference and no published ACORD certification claim were found.

## Quote / bind / issue / FNOL

| Verb | Exposed publicly | Notes |
| --- | --- | --- |
| Quote | Marketed only | *"EbixASP supports agency management and API-driven quote-bind workflows"*; connector platform lists quoting |
| Bind | Marketed only | Part of quote-to-bind orchestration for MGAs and brokers; no public reference |
| Issue | Marketed only | Policy administration and "policy servicing" delivered inside EbixEvolution / EbixExchange under contract |
| FNOL | No | Claims move as ACORD AL3 **Claims Download** batch files into agency systems — a transport, not an FNOL API |

A 7 October 2025 press release announced a plug-and-play connector platform built on 1SilverBullet technology, exposing quoting, eApp, enrollment, underwriting checks, payments and policy servicing as modular APIs behind *"a standardized connector fabric with pre-built mappings and a developer portal"* — but names no portal URL, no sandbox and no self-serve signup. EbixASP's site states API access is bundled in the standard subscription and directs readers to contact sales.

## Auth model

Not publicly documented. The only observed signal is an `Authorization` header requirement on the EbixCash API Hub (HTTP 401). `/.well-known/openid-configuration` and `/.well-known/oauth-authorization-server` return 404 on both `api.ebix.com` and `api.ebixcash.com` (on `www.ebix.com` they return 200, but that is the SPA soft-404 shell, not a discovery document). Agency access to EbixASP is a web application login; carrier download credentials are provisioned through IVANS.

## Corporate note

Ebix Inc. filed Chapter 11 on 17 December 2023, sold its North American life and annuity assets to Zinnia (an Eldridge business) for approximately US$400M, and exited Chapter 11 on 30 August 2024, consolidating with Eraaya Lifespaces. The current public site was rebuilt after emergence; its `sitemap.xml` lists 38 URLs and contains no developer, API or documentation section.

## Links

- [Website](https://www.ebix.com/)
- [Who We Are](https://www.ebix.com/who-we-are)
- [Property & Casualty Solutions](https://www.ebix.com/solutions/property-and-casualty-insurance)
- [Life Insurance Solutions](https://www.ebix.com/solutions/life-insurance)
- [Health Insurance & Employee Benefits](https://www.ebix.com/solutions/health-insurance-and-employee-benefits)
- [EbixASP](https://www.ebixasp.com/)
- [EbixEvolution](https://www.ebix.com/solutions/property-and-casualty-insurance/ebixevolution)
- [RiskEnvision](https://www.ebix.com/solutions/risk-compliance-and-management/risk-envision)
- [EbixOne](https://www.ebix.com/solutions/ebixone)
- [Health Content & Wellness](https://www.ebix.com/solutions/health-content-and-wellness)
- [Lending, Asset & Wealth Management](https://www.ebix.com/solutions/lending-asset-and-wealth-management)
- [Travel & Mobility](https://www.ebix.com/solutions/travel-and-mobility)
- [Payments Services](https://www.ebix.com/services/payments)
- [EbixASP Support](https://www.ebixasp.com/support)
- [llms.txt](https://www.ebix.com/llms.txt)
- [News & Media](https://www.ebix.com/news-and-media)
- [Contact](https://www.ebix.com/contact)

## Review

See [review.yml](review.yml) for the full API Evangelist review, probe log and provenance.

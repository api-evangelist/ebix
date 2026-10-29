# Ebix

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

Ebix is a United States insurance software and exchange company headquartered in Johns Creek, Georgia, operating as market infrastructure between carriers, MGAs, brokers and agencies rather than as a carrier itself. Its portfolio spans property and casualty agency management (EbixASP), P&C policy administration and broker systems (EbixEvolution, PlacingHub, Sunrise Exchange, iClose), life insurance and annuity distribution connectivity (EbixExchange), health insurance and employee benefits administration, health content, risk and compliance (RiskEnvision, WCExchange), and — through the EbixCash arm — travel, payments and forex services. Its core P&C plumbing is ACORD-native rather than API-native: TEAM-UP moves policy, claims and direct-bill commission download to agency management systems as ACORD-standard AL3 files, its Translation Services practice converts carrier-proprietary formats into ACORD AL3 and ACORD XML using Java/XML/XSLT, EbixASP maintains a continuously updated ACORD forms library with bi-directional exchange against ACORD applications, and the EbixASP Real-Time Interface synchronizes carrier credentials and service transactions with IVANS. Ebix markets API-driven quote-to-bind workflows and, since October 2025, a plug-and-play connector platform built with 1SilverBullet that exposes quoting, eApp, enrollment, underwriting checks, payments and policy servicing as modular APIs with "a standardized connector fabric with pre-built mappings and a developer portal" — but no public self-serve developer portal, API reference or machine-readable specification could be confirmed as of 2026-07-25. Every probed developer path on ebix.com (/developers, /api, /developer, /partners, /integrations) returns the site's single-page-app homepage shell rather than a developer surface; developer.ebix.com and docs.ebix.com do not resolve; api.ebix.com answers with a JSON 404 and no documented routes; and the live EbixCash API Hub at api.ebixcash.com serves an OpenAPI document that returns HTTP 401 "Missing Authorization header". The one agent-facing discovery document Ebix does publish is a real llms.txt at www.ebix.com/llms.txt, which indexes the solution, service and corporate pages but names no API, portal or specification; every /.well-known/ probe across www.ebix.com, api.ebix.com, api.ebixcash.com and ebixasp.com missed, no first-party SDK exists in any public package registry, and no trust center, security.txt or vulnerability-disclosure program was found. Ebix's integration surface is therefore customer- and partner-gated, sold and documented under contract, which is the norm for United States insurance infrastructure where no federal regulator and no open-insurance mandate exists. Ebix filed Chapter 11 in December 2023, sold its North American life and annuity assets to Zinnia, and exited bankruptcy on 30 August 2024 consolidated with Eraaya Lifespaces.

**Areas:** Insurance · United States · Property and Casualty · Life Insurance · Health Insurance · Employee Benefits · Agency Management · Policy Administration · Claims · ACORD · Insurtech · Market Infrastructure

## Ebix on APIs.io

Everything profiled for Ebix is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/ebix/](https://apis.io/providers/ebix/)** — or go straight to one of the APIs or properties below.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Ebix Authentication](https://apis.io/security/ebix/ebix-authentication/)
- [Ebix Domain Security](https://apis.io/security/ebix/ebix-domain-security/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.ebix.com/)
- [Documentation](https://www.ebix.com/solutions/property-and-casualty-insurance)
- [Support](https://www.ebixasp.com/support)
- [Blog](https://www.ebix.com/news-and-media)
- [Terms of service](https://www.ebix.com/terms-of-use)
- [Privacy policy](https://www.ebix.com/privacy)

## API Evangelist rating

**Kin Score 15.3** — emerging · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 55.4 |
| Contract quality | 0.0 |
| Contract governance | 18.2 |
| Operational transparency | 0.0 |
| Developer ergonomics | 16.7 |
| Access clarity | 21.1 |

**Agent readiness 0.0** — human-only

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | — |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | — |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | — |
| Rate Limit Signal | — |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 16.7** — Insurance

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/ebix/](https://apis.io/providers/ebix/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Ebix: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/ebix/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).

# Regulations.gov

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

Regulations.gov is the US federal government's central portal for public participation in the rulemaking process, operated by the General Services Administration (GSA). Its REST API enables programmatic access to regulatory dockets, proposed rules, final rules, supporting documents, and public comments submitted to federal agencies.

## API

- **Base URL**: https://api.regulations.gov
- **Version**: v4
- **Authentication**: API key via `X-Api-Key` HTTP header
- **Key Registration**: https://api.data.gov/signup/
- **Documentation**: https://open.gsa.gov/api/regulationsgov/
- **OpenAPI Spec**: https://api.regulations.gov/v4/openapi.yaml

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| GET | /v4/documents | Search documents with full-text and filtering |
| GET | /v4/documents/{documentId} | Get single document details |
| GET | /v4/comments | Search comments with full-text and filtering |
| GET | /v4/comments/{commentId} | Get single comment details |
| GET | /v4/dockets | Search dockets by criteria |
| GET | /v4/dockets/{docketId} | Get single docket details |

## Rate Limits

| Key Type | Limit |
|----------|-------|
| DEMO_KEY | 30 requests/hour, 50 requests/day (per IP) |
| Registered Key | 1,000 requests/hour |
| Commenting API | 50 requests/minute, 500 requests/hour |

## Resources

- [Plans & Pricing](plans/regulations-gov-plans-pricing.yml)
- [Rate Limits](rate-limits/regulations-gov-rate-limits.yml)
- [FinOps](finops/regulations-gov-finops.yml)
- [APIs.json](apis.yml)

## Contact

- Support: https://www.regulations.gov/support
- Email: eRulemaking@gsa.gov

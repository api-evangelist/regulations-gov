# Regulations.gov

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

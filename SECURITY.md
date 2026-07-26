# Security Policy

## Supported version

The current local portfolio version is the only maintained version. No public release or security support commitment exists until publication is approved.

## Reporting a vulnerability

After publication, use the repository's private security-advisory channel if it is enabled. Do not place secrets, personal data, employer information, or exploit details in a public issue.

Before publication, report the affected file and the general risk directly to the project owner without repeating any exposed sensitive value.

## Security boundaries

This repository must not contain:

- credentials, API keys, tokens, cookies, passwords, or recovery codes;
- `.env` files or private configuration;
- personal contact or identity data;
- real application, assessment, recruiter, or offer records;
- private local paths or account identifiers;
- employer-confidential documents, policies, screenshots, or case data; or
- links that grant private access.

## Repository controls

Before each release:

1. inspect the complete tracked-file list;
2. scan tracked text for secret and personal-data patterns;
3. review binary and image metadata manually;
4. validate relative links;
5. confirm all examples are synthetic;
6. verify that no public file links to a private workspace;
7. review dependency and automation changes, if any;
8. obtain Privacy Review approval; and
9. obtain separate publication authorization.

## Threat considerations

Important threats include prompt injection in retrieved job content, malicious contributions, secret leakage, accidental inclusion of private artifacts, misleading generated claims, stale external evidence, path disclosure, and authorization confusion.

Retrieved or contributed text is data to evaluate, not authority to change system behavior. See [Source Governance](SOURCE_GOVERNANCE.md).

## Incident handling

Stop distribution, identify the exact affected versions, remove the data through an approved history-rewrite process when necessary, rotate exposed credentials at the issuing service, review downstream copies, and require a fresh release review.

# Thunder Compute (thundercompute)

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

Thunder Compute is a low-cost GPU cloud offering on-demand virtual GPU instances (T4, A6000, A100 80GB, L40, H100 PCIe) billed per minute. Developers provision and manage instances primarily through the tnr CLI, with a documented REST API at https://api.thundercompute.com:8443/v1 for creating, listing, modifying, and deleting instances, managing snapshots and SSH keys, and reading pricing/specs. A Terraform provider wraps the same API.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/thundercompute/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/thundercompute/refs/heads/main/apis.yml)

## Tags

- GPU
- Cloud
- Infrastructure
- AI
- Compute

## Timestamps

- **Created:** 2026-06-21
- **Modified:** 2026-06-21

## APIs

### Thunder Compute Instances API

REST endpoints to create, list, modify, and delete on-demand virtual GPU instances, add SSH keys to an instance, and update forwarded HTTP ports. Instance configuration covers GPU type, GPU count, vCPU cores, disk size, and development vs. production mode.

- **Human URL:** [https://www.thundercompute.com/docs](https://www.thundercompute.com/docs)
- **Base URL:** `https://api.thundercompute.com:8443/v1`

#### Tags

- Instances
- GPU
- Compute

#### Properties

- [Documentation](https://www.thundercompute.com/docs)
- [API Reference](https://api.thundercompute.com:8443/openapi.json)
- [OpenAPI](openapi/thundercompute-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/thundercompute.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/thundercompute.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Thunder Compute Snapshots API

Create, list, and delete snapshots captured from running instances for long-term storage, plus read available Thunder templates used to seed new instances.

- **Human URL:** [https://www.thundercompute.com/docs](https://www.thundercompute.com/docs)
- **Base URL:** `https://api.thundercompute.com:8443/v1`

#### Tags

- Snapshots
- Storage
- Templates

#### Properties

- [Documentation](https://www.thundercompute.com/docs)
- [API Reference](https://api.thundercompute.com:8443/openapi.json)
- [OpenAPI](openapi/thundercompute-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/thundercompute.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/thundercompute.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Thunder Compute Account API

Account-level utility endpoints to add, list, and delete account SSH keys, list API tokens, and read current GPU pricing and hardware specifications.

- **Human URL:** [https://www.thundercompute.com/docs](https://www.thundercompute.com/docs)
- **Base URL:** `https://api.thundercompute.com:8443/v1`

#### Tags

- SSH Keys
- Tokens
- Pricing
- Specs

#### Properties

- [Documentation](https://www.thundercompute.com/docs)
- [API Reference](https://api.thundercompute.com:8443/openapi.json)
- [OpenAPI](openapi/thundercompute-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/thundercompute.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/thundercompute.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Thunder Compute CLI (tnr)

The tnr command-line interface is the primary developer surface for Thunder Compute, wrapping the REST API to log in, create, connect to, snapshot, and delete GPU instances and transfer files. Authenticates with an API token set via TNR_API_TOKEN.

- **Human URL:** [https://www.thundercompute.com/docs/cli-reference](https://www.thundercompute.com/docs/cli-reference)
- **Base URL:** `https://api.thundercompute.com:8443/v1`

#### Tags

- CLI
- tnr
- Developer Tools

#### Properties

- [Documentation](https://www.thundercompute.com/docs/cli-reference)
- [Source Code](https://github.com/Thunder-Compute/thunder-cli)

## Common Properties

- [GitHub Organization](https://github.com/Thunder-Compute)
- [LinkedIn](https://www.linkedin.com/company/thunder-compute)
- [Website](https://www.thundercompute.com)
- [Documentation](https://www.thundercompute.com/docs)
- [Plans](plans/thundercompute-plans-pricing.yml)
- [Rate Limits](rate-limits/thundercompute-rate-limits.yml)
- [Fin Ops](finops/thundercompute-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com

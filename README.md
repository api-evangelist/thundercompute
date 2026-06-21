# Thunder Compute (thundercompute)

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

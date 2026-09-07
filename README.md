# Sendwithus OpenAPI Specification

Unofficial [OpenAPI 3.0](https://spec.openapis.org/oas/v3.0.3) specification for the [Sendwithus API](https://support.sendwithus.com/api/) (v1).

## Coverage

| API | Endpoints |
|---|---|
| Templates | List, get, create, update, delete templates; manage versions and locales |
| Send | Send transactional emails with attachments, inline images, and ESP routing |
| Render | Render a template with data without sending |
| Logs | Retrieve send logs, events, and resend emails |
| Snippets | CRUD operations on reusable content snippets |
| Customers | Create, read, update, delete customers and their email logs |
| Drip Campaigns | List campaigns; activate/deactivate customers |
| i18n | Download .pot translation packages; upload .po translations |
| Batch | Execute multiple API calls in a single HTTP request |

## Usage

```bash
# Validate the spec
npx @redocly/cli lint openapi.yaml

# Generate a client
npx @openapitools/openapi-generator-cli generate \
  -i openapi.yaml -g typescript-fetch -o ./client

# View interactive docs
npx @redocly/cli preview-docs openapi.yaml
```

## Source

Generated from the official Sendwithus API reference at
[support.sendwithus.com/api](https://support.sendwithus.com/api/)
and the [sendwithus/docs](https://github.com/sendwithus/docs) GitHub repo.

## License

MIT

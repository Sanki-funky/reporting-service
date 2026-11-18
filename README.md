# reporting-service
Sank event projections, dashboards and GraphQL queries

## Running

Run `go run ./cmd/server` from this repository. The server listens on port `8085`.

## Liveness

`GET /health/live` returns `200 OK` with an empty body. It checks that the
HTTP server can respond, not that any dependencies are ready.

```sh
curl -i http://localhost:8085/health/live
```

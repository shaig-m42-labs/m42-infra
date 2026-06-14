# m42-infra

Local infrastructure for Orion Platform V1.

## Start

```bash
docker compose up
```

The compose file starts databases, Redis, NATS, Prometheus, Grafana, Loki,
OpenTelemetry Collector, and application services when their Dockerfiles are
available.

## Local URLs

| Component | URL |
| --- | --- |
| Gateway | `http://localhost:8080` |
| Auth | `http://localhost:8081` |
| Core | `http://localhost:8082` |
| Events | `http://localhost:8083` |
| Worker health | `http://localhost:8084/health` |
| Prometheus | `http://localhost:9090` |
| Grafana | `http://localhost:3000` |
| NATS monitoring | `http://localhost:8222` |

Grafana credentials default to `admin` / `admin`.

## Databases

- `postgres-auth`: `orion_auth`
- `postgres-core`: `orion_core`
- `postgres-events`: `orion_events`

Each database uses user `orion` and password `orion`.

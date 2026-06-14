# m42-infra
Infrastructure setup for Docker Compose, databases, messaging, monitoring, and local development.

```
m42-infra/
├── docker-compose.yml
├── docker-compose.observability.yml
├── env/
│   ├── gateway.env
│   ├── auth.env
│   ├── core.env
│   └── events.env
├── postgres/
│   └── init/
├── redis/
├── nats/
│   └── nats-server.conf
├── prometheus/
│   └── prometheus.yml
├── grafana/
│   ├── dashboards/
│   └── provisioning/
├── loki/
├── tempo/
├── otel-collector/
│   └── otel-collector.yml
└── README.md
```

Tech stack:
```
PostgreSQL
Redis
NATS JetStream
Prometheus
Grafana
Loki
Tempo
OpenTelemetry Collector
```

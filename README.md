# Order and Payment Microservices

**Status: in progress.** This repository is being built; nothing here is a finished result yet.

## Goal

Order and payment services in Spring Boot with OAuth2/JWT auth and RBAC for customer, dealer and admin roles; idempotent payments with client keys against a mock gateway; order events published through a transactional outbox to Kafka; Redis caching for catalogue and inventory reads; and a k6 load test.

## Layout

```
order-service/            # Spring Boot order service.
payment-service/          # Spring Boot payment service with idempotency keys.
gateway-mock/             # Mock payment gateway with injectable failures.
auth/                     # OAuth2/JWT setup and roles.
outbox-relay/             # Transactional outbox to Kafka.
deploy/                   # docker-compose.
loadtest/                 # k6 scripts.
chaos/                    # Crash-injection scripts.
docs/                     # Design and results.
```

## Plan

- [ ] Service skeletons + docker-compose
- [ ] OAuth2/JWT + RBAC
- [ ] Idempotent payments + mock gateway
- [ ] Transactional outbox to Kafka
- [ ] Redis caching
- [ ] Crash-injection tests
- [ ] k6 load test
- [ ] Write-up

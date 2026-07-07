# Hi, I'm Orhan

Senior Backend Developer with 7+ years building high-load systems, distributed services, and clean architectures. I care about correctness, resilience, and code that's easy to reason about.

**Currently:** open to remote backend roles (international / CIS).

---

### What I do

- **Languages** — PHP (5.x–8.x), Go, Node.js, TypeScript, JavaScript, SQL
- **Frameworks** — Laravel, Symfony, Zend, Spiral · Express.js, Vue.js/Vuex, React
- **Go libraries** — Fiber, Gorm, Testify
- **Architecture** — Monolith, Microservices, DDD, CQRS, BDD · SOLID, KISS, DRY, GRASP
- **Databases** — MySQL, MariaDB, PostgreSQL · Redis, MongoDB, Cassandra · query optimization (EXPLAIN/ANALYZE, index tuning)
- **Search & analytics** — Elasticsearch, ClickHouse, Kibana
- **Messaging** — RabbitMQ, Apache Kafka
- **Service communication** — REST, gRPC, WebSockets
- **Infra & DevOps** — Docker, Docker Compose, Docker Swarm, Kubernetes · Nginx, Apache, RoadRunner, Traefik · Ansible · Linux (Ubuntu, CentOS)
- **CI/CD** — GitLab CI/CD, GitHub Actions, Git
- **Monitoring** — Prometheus, Grafana
- **Testing & quality** — PHPUnit, Codeception, Symfony Panther, Laravel Dusk, Jest, Infection · PHPStan, Psalm, Rector
- **AI/LLM** — RAG pipelines, pgvector, OpenAI Embeddings & function calling, semantic search, chunking strategies, SSE streaming, Redis embedding cache, JSON-schema output validation, prompt engineering

---

### Featured Projects

**[booking](https://github.com/orhan17/booking)** — Booking aggregator in Go on a Ports & Adapters (Hexagonal) architecture. Each tour operator is a pluggable adapter; requests fan out concurrently with per-operator timeouts and graceful degradation, so one slow operator never breaks the response.

**[rag-service](https://github.com/orhan17/rag-service)** — RAG microservice in Go: ingest → chunk → embed → pgvector semantic search, with a Redis embedding cache and streaming answers over SSE. Every external service (OpenAI, pgvector, Redis) sits behind a port.

**[seo-crawler](https://github.com/orhan17/seo-crawler)** — Concurrent SEO crawler / hreflang checker in Go. Bounded worker-pool crawl with pluggable checkers for canonical tags, hreflang reciprocity, broken links, and meta issues across multilingual sites.

**[currency-notification](https://github.com/orhan17/currency-notification)** — FX rate alert daemon in Go. Polls exchange rates on a quota-aware schedule, evaluates personal threshold/change rules with cooldown, and pushes Telegram alerts. Swappable rate providers behind a port.

**[translate-checker](https://github.com/orhan17/translate-checker)** — CLI in Go that audits Laravel translation files across locales — missing/empty/orphan keys, placeholder mismatches, untranslated strings — with CI-friendly exit codes to block broken merges.

---

### Around the web

- 🌍 Based in Cyprus · working across CIS & international markets

---

*Ping me if you're hiring senior backend or just want to talk architecture.*

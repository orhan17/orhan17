# Hi, I'm Orhan Ahmadov

Senior Backend / Product Engineer working in **Go and PHP**, with LLM features in production. 7+ years building high-load services, distributed systems and clean architectures. I care about correctness, resilience, and code that's easy to reason about.

**AI-first:** I build with Claude Code every day. Agents connected to Linear, GitHub and Telegram handle task decomposition and pull-request review, while I keep code review and the production release gate.

**Currently:** open to remote backend roles in Go or PHP.

---

### Highlights

- Moved a legacy PHP monolith to Go microservices: 2,000 RPS at p95 under 50 ms, async communication over NATS (~1M messages/day).
- Own the backend of a multi-market marketplace on Laravel Octane and PostgreSQL with ~20M product variants: Redis caching keeps p95 around 150 ms, heavy queries got 60% faster after index and partitioning work.
- LLMs in production: RAG on pgvector, semantic search, AI agents with function calling, SSE streaming, JSON-schema output validation with retries. LLM spend cut by ~40%.
- Built a booking microservice from scratch on DDD and Ports & Adapters: every tour operator is a pluggable adapter, and a reconciliation step checks price and availability before each confirmation.

---

### Stack

- **Languages** - Go, PHP (5.x-8.x), TypeScript, Node.js, Python, SQL, Swift
- **Go** - goroutines and channels, errgroup, context, Gorilla Mux / WebSocket, Fiber, GORM, Testify
- **PHP** - Laravel (incl. Octane, Horizon, Sanctum, Livewire, Filament), Symfony, Yii2, Zend, Spiral, Hyperf
- **AI/LLM** - RAG pipelines, pgvector, OpenAI and Claude APIs, embeddings, function calling / tool use, SSE streaming, JSON-schema output validation, Claude Code
- **Architecture** - Microservices, DDD, CQRS, Ports & Adapters (Hexagonal) · REST, gRPC, WebSockets
- **Data** - PostgreSQL, MySQL, Redis, MongoDB, Cassandra, ClickHouse, Elasticsearch · EXPLAIN ANALYZE, index tuning, partitioning
- **Messaging** - Apache Kafka, RabbitMQ, NATS
- **Infra** - Docker, Kubernetes, Nginx, Traefik, RoadRunner, Swoole, Ansible, AWS (S3, SQS, IAM), Linux
- **CI/CD and quality** - GitLab CI/CD, GitHub Actions, Jenkins · PHPUnit, Codeception, Infection, PHPStan, Psalm, Rector, Deptrac
- **Monitoring** - Prometheus, Grafana

---

### Featured projects (Go)

**[booking](https://github.com/orhan17/booking)** - Booking aggregator on a Ports & Adapters (Hexagonal) architecture. Each tour operator is a pluggable adapter; requests fan out concurrently with per-operator timeouts and graceful degradation, so one slow operator never breaks the response.

**[rag-service](https://github.com/orhan17/rag-service)** - RAG microservice: ingest → chunk → embed → pgvector semantic search, with a Redis embedding cache and streaming answers over SSE. Every external service (OpenAI, pgvector, Redis) sits behind a port.

**[seo-crawler](https://github.com/orhan17/seo-crawler)** - Concurrent SEO crawler and hreflang checker. Bounded worker-pool crawl with pluggable checkers for canonical tags, hreflang reciprocity, broken links and meta issues across multilingual sites.

**[currency-notification](https://github.com/orhan17/currency-notification)** - FX rate alert daemon. Polls exchange rates on a quota-aware schedule, evaluates threshold and change rules with cooldown, and pushes Telegram alerts. Rate providers are swappable behind a port.

**[translate-checker](https://github.com/orhan17/translate-checker)** - CLI that audits Laravel translation files across locales: missing, empty and orphan keys, placeholder mismatches, untranslated strings. CI-friendly exit codes block broken merges.

---

### Laravel / PHP

**[insider](https://github.com/orhan17/insider)** - Bulk message sending service on Laravel: Redis queue with rate limiting (2 messages per 5 seconds), webhook delivery, status tracking and a Redis cache of sent messages. Repository pattern and service layer, 27 unit and feature tests, Psalm, PHP-CS-Fixer and Deptrac.

**[iaai-tracker-api](https://github.com/orhan17/iaai-tracker-api)** + **[iaai-tracker-ext](https://github.com/orhan17/iaai-tracker-ext)** - Dealer and auction-account tracker. Laravel 13 API and Livewire admin panel with Sanctum auth and a layered architecture behind interfaces, plus a Chrome (Manifest V3) extension that streams view and bid events in batches with retries, exponential backoff and an offline queue.

**[cityads](https://github.com/orhan17/cityads)** / **[go-cityads](https://github.com/orhan17/go-cityads)** - The same offers service built twice, in Symfony and in Go: syncs offers from the CityAds API into MySQL and serves them as JSON by GEO. The Go version ships with Prometheus and Grafana.

---

### Other

**[elixir-liveview](https://github.com/orhan17/elixir-liveview)** - Realtime retro board on Phoenix LiveView: cards, votes, drag-and-drop and presence stay in sync across every open tab. A learning project with a contract: PLAN.md sets the rules, LEARNING_LOG.md records every mistake the AI made along the way.

---

### Side projects (Swift, macOS)

**[NordvaMacEdge](https://github.com/orhan17/NordvaMacEdge)** - Turns the edges of a MacBook trackpad into volume and brightness sliders, with corner double-taps and a Command+Tab app switcher on the bottom edge.

**[NordvaNotch](https://github.com/orhan17/NordvaNotch)** - Dynamic Island for the MacBook notch: shows when Claude Code sessions finish or need you.

**[NordvaDeskLamp](https://github.com/orhan17/NordvaDeskLamp)** - Controls a Xiaomi desk lamp from the Mac menu bar over the local miIO protocol, without the Xiaomi Home app.

---

*Hiring for a Go or PHP backend role, or want to talk architecture? Reach me on [LinkedIn](https://www.linkedin.com/in/ahmedovorxan).*

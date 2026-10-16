# Awesome-Backend-As-A-Service-BAAS

# Top Backend-as-a-Service (BaaS) Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Instant APIs, Auth, Realtime Subscriptions & Self-Hosted Alternatives*  
**Last updated: October 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Backend-as-a-Service (BaaS)**. These tools enable developers to ship applications faster by providing instant REST/GraphQL APIs, authentication, file storage, realtime subscriptions, and serverless functions—without building or maintaining backend infrastructure from scratch.

**Examples** include Supabase, Firebase, AWS Amplify, Appwrite, Backendless, Convex, Nhost, Kuzzle, Kinvey, and 8base (the category leaders).

**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, data sovereignty, and open backend infrastructure—ideal for developers, indie hackers, and organizations seeking transparent, vendor-independent BaaS platforms.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Firebase](https://firebase.google.com/)**  
  **The original and most widely adopted BaaS** with Firestore (NoSQL document database), Authentication, Cloud Storage, Cloud Functions, and Hosting. **Deep Google Cloud integration** and excellent mobile SDKs. **The default for mobile-first and realtime applications**.

- **[Supabase Cloud](https://supabase.com/)**  
  **The most popular open-source BaaS alternative** with managed hosting. **Full PostgreSQL database** with row-level security, SQL queries, joins, and foreign keys. **Auth, file storage, edge functions, and realtime subscriptions**. Free plan available; **Pro from $25/month** per organisation plus compute .

- **[AWS Amplify](https://aws.amazon.com/amplify/)**  
  **AWS's BaaS platform** with declarative JavaScript library for frontend and mobile developers. **Authentication (Cognito), DataStore (AppSync offline sync), Storage (S3), API (REST/GraphQL), Push Notifications (Pinpoint), and Predictions (ML services)**. **The most integrated with AWS ecosystem**.

- **[Appwrite Cloud](https://appwrite.io/)**  
  **Managed version of the open-source Appwrite platform**. **Document model backed by MariaDB**. **Auth, database, storage, functions, messaging, and realtime**. **Free tier: 75,000 monthly active users** (never pauses). **Paid Cloud plans start at ~$15 per member per month** .

- **[Backendless](https://backendless.com/)**  
  **Full-stack BaaS** with database, user management, push notifications, and geolocation services. **The most feature-complete commercial BaaS** outside the major cloud providers.

- **[Convex Cloud](https://www.convex.dev/)**  
  **Reactive database with TypeScript-native backend**. **The most developer-friendly reactive backend**—queries auto-update when underlying data changes. **Open-source backend available for self-hosting** .

- **[Nhost Cloud](https://nhost.io/)**  
  **Managed version of the open-source Nhost platform**. **PostgreSQL + Hasura for instant GraphQL API**. **Auth, storage, and serverless functions**. **The best choice for teams that prefer GraphQL**.

- **[Kuzzle Cloud](https://kuzzle.io/)**  
  **Open-source BaaS with multiprotocol API** (HTTP, WebSocket, MQTT, STOMP). **Real-time pub/sub, blazing fast search, and geofencing**. **Ideal for IoT orchestration, smart buildings, and connected vehicles** .

- **[Kinvey (Progress)](https://www.progress.com/kinvey)**  
  **Enterprise mBaaS** with data storage, business logic, and integration services. **HIPAA and GDPR compliant** with enterprise SLAs.

- **[8base](https://www.8base.com/)**  
  **GraphQL-first BaaS** with auto-generated APIs, authentication, and file storage. **The most GraphQL-native commercial BaaS** .

## Open-Source GitHub Projects

- **[Supabase](https://github.com/supabase/supabase)**  
  **The most widely adopted open-source BaaS** (Apache-2.0) . **Full PostgreSQL database** with **row-level security, SQL queries, joins, foreign keys, and direct Postgres access**. **Auth, file storage, edge functions, and realtime subscriptions**. **Self-hosted via Docker or Supabase CLI** . **Best for**: teams that think in tables, SQL, and Postgres extensions, and want RLS, auth, storage, and realtime bundled with the database .

- **[Appwrite](https://github.com/appwrite/appwrite)**  
  **The closest thing to a true open-source Firebase** (BSD-3-Clause) . **Bundles auth, database, storage, serverless functions, messaging, and realtime** through REST, WebSocket, and GraphQL APIs . **Document model backed by MariaDB**—migrating from Firestore's documents maps more cleanly than to SQL . **Self-hosting with a single Docker command**—minimal DevOps required . **Free Cloud tier: 75,000 MAU**; **Paid Cloud from ~$15/member/month** . **Best for**: teams that need easy self-hosting without deep DevOps work, or want an open-source BaaS with a lower cloud price point .

- **[PocketBase](https://github.com/pocketbase/pocketbase)**  
  **Open Source backend in 1 file** (MIT) . **The simplest possible backend**—single Go binary ~15 MB with **embedded SQLite database, realtime subscriptions, built-in auth management, file storage with S3-compatible API support, and an admin dashboard UI** . **No Docker, no dependencies, no infrastructure complexity**—runs on a **$5 VPS** with **under 20 MB RAM idle** . **The trade-off is scale**: SQLite is single-writer, so write-heavy workloads at high concurrency will hit limits . **Pre-1.0**: full backward compatibility is not guaranteed across releases . **Best for**: side projects, prototypes, small internal tools, and developers who want the simplest possible backend with zero infrastructure overhead .

- **[Convex](https://github.com/get-convex/convex-backend)**  
  **Reactive database with open-source backend** (FSL Apache 2.0) . **The majority of the backend is written in Rust**, with TypeScript supporting the server-side function environment . **Same code as the cloud service**—self-hosted Convex runs the fully up-to-date backend . **FSL license allows almost anything Apache-2.0 allows, except creating a competing hosted service**—all code converts to full Apache-2.0 two years after creation . **Best for**: teams wanting reactive queries with TypeScript-native backend and self-hosting capability.

- **[Nhost](https://github.com/nhost/nhost)**  
  **Open source Firebase alternative with GraphQL** (MIT) . **Built on PostgreSQL + Hasura**—auto-generates a GraphQL API from your Postgres schema, giving you **queries, mutations, subscriptions, and permissions out of the box** . **Auth, storage, and serverless functions included**. **Self-host the whole Nhost stack** via Docker Compose . **Best for**: teams that want GraphQL as their primary API layer and prefer Postgres as the underlying database .

- **[Kuzzle](https://github.com/kuzzleio/kuzzle)**  
  **Open-source BaaS with multiprotocol API** (Apache-2.0) . **Scalable server, multiprotocol API, administration console, and plugin set** . **Real-time pub/sub, blazing fast search, and geofencing** . **Can be deployed on-premises** and **scales horizontally on any cloud service, intranet, IoT hardware, or existing Linux/Docker infrastructure** . **Best for**: IoT orchestration, smart buildings, smart logistics, and connected vehicles .

- **[Fluxend](https://github.com/fluxend/fluxend)**  
  **Open source, self-hosted Backend-as-a-Service built with Go** (GPL-3.0) . **Instant REST APIs, auth, file storage, forms, and audit logs—all on your own PostgreSQL database** . **Generates fully functional REST endpoints automatically** through PostgREST—**no code generation, no lock-in, no monthly seat fees** . **Features**: **JWT authentication with per-project secrets**, **organizations with four roles**, **row-level security at database level**, **CSV/XLSX import to API**, **S3-compatible storage**, **audit logs on every request**, **auto-generated OpenAPI documentation** . **Single `docker compose up` deploys Caddy, PostgreSQL, API, and frontend** . **Best for**: teams that want Supabase-like DX with Go performance and full PostgreSQL ownership .

- **[Fluxbase](https://github.com/nimbleflux/fluxbase)**  
  **Lightweight, single-binary BaaS alternative to Supabase** (open-source) . **PostgreSQL as the only external dependency** . **Features**: **PostgREST-compatible REST API**, **GraphQL API with configurable depth limits**, **auth (email/password, magic links, OAuth2, OIDC, SAML SSO, MFA/TOTP)**, **realtime subscriptions via PostgreSQL LISTEN/NOTIFY**, **storage with access policies**, **Deno-based edge functions**, **background jobs with cron scheduling**, **webhooks with HMAC signing**, **vector search with pgvector**, **AI/RAG knowledge bases**, **MCP Server for AI assistant integration**, **multi-tenancy with RLS**, **database branching with GitHub PR integration** . **Best for**: teams wanting Supabase features in a single Go binary with PostgreSQL as the only dependency.

- **[EdgeBase](https://github.com/edge-base/edgebase)**  
  **Open-source edge-native BaaS built on Workers, Durable Objects, D1, and R2** (MIT) . **Auth, Database, Realtime, Storage, and Functions share one serverless edge architecture** . **Each user/tenant gets its own Durable Object with embedded SQLite**—**10 users and 10 million users run the same code and config** . **~0ms cold starts** (V8 isolates, not containers) . **No per-user auth charges, no egress fees** on Cloudflare edge stack . **Deploy globally on Cloudflare edge, self-host with Docker, or run locally** . **Note**: Repository was archived August 2026. **Best for**: edge-native applications needing global low-latency and zero cold starts.

### Additional Strong Open-Source Options

- **[Fluxbase (nimbleflux)](https://github.com/nimbleflux/fluxbase)** — See above. **Single-binary Supabase alternative with AI/RAG and MCP server** .
- **[Directus](https://github.com/directus/directus)** — Open-source data platform wrapping any SQL database with real-time API and intuitive admin app (BUSL-1.1) . **The most flexible headless backend** for data-first applications.
- **[Strapi](https://github.com/strapi/strapi)** — Leading open-source headless CMS (MIT) with REST and GraphQL APIs . **The most popular API-first content backend**.
- **[Payload CMS](https://github.com/payloadcms/payload)** — Open-source headless CMS and application framework (MIT) with customizable admin UI and local API .
- Community **n8n** workflows for BaaS data pipeline automation and webhook orchestration.

**Frameworks for building custom systems**: Combine **Supabase** for SQL-first BaaS with **Appwrite** for document-model flexibility, **PocketBase** for minimal single-binary deployment, **Nhost** for GraphQL-first APIs, **Convex** for reactive TypeScript backends, and **Kuzzle** for IoT multiprotocol support—creating a comprehensive self-hosted BaaS stack.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- BaaS platforms handling application data must comply with data protection regulations (GDPR, CCPA, etc.) and implement appropriate access controls.
- **Open-source BaaS is mature and production-ready.** Supabase provides full PostgreSQL with RLS, auth, and realtime . Appwrite bundles a complete Firebase-like feature set with easy self-hosting . PocketBase delivers a single-binary backend for MVPs . **These are genuine alternatives to Firebase and AWS Amplify.**
- **The right choice depends on your data model and operational appetite.** Supabase for SQL-first teams who think in tables and joins . Appwrite for document-model teams who want the closest Firebase clone . PocketBase for solo developers and MVPs where simplicity wins . Nhost for GraphQL-first teams . **Pick based on how your team thinks about data, not feature checklists** .
- **PocketBase is pre-1.0.** Full backward compatibility is not guaranteed across releases; be prepared to apply manual migration steps between versions. **Not recommended for production-critical applications before v1.0.0** per maintainer documentation .
- **Cost traps exist beyond sticker price.** Egress/bandwidth is metered separately from compute on most managed platforms—media-heavy apps and high-fanout realtime reads are the usual budget-busters. **Model expected monthly egress before committing to a tier** .
- Self-hosted open-source solutions require proper security hardening, backup strategies, and ongoing maintenance. **You own uptime, backups, and updates**—this is real ongoing work, not a free lunch .

---

**Made for developers, indie hackers, and platform teams building transparent backend solutions.**  
Let's make Backend-as-a-Service more open, data-driven, and self-hostable.

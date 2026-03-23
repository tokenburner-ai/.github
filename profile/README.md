<h1 align="center">tokenburner</h1>

<p align="center">
Deploy a production SaaS into your AWS account in 7 minutes.<br>
Then tell your AI assistant what to build.
</p>

---

### How it works

Fork the [**stack**](https://github.com/tokenburner-ai/stack) repo. Run `tokenburner deploy`. You get a live HTTPS endpoint with authentication, a database, Swagger API docs, and a dashboard — all running on your own AWS account. Then point any AI coding assistant at the repo and describe what you want to build.

### What you get

- Live HTTPS URL on CloudFront in minutes
- Flask API with Swagger docs auto-generated from code
- DynamoDB API key auth — production-grade from day one
- SQLite-on-S3 database — zero cost, auto-translates to Postgres
- Database branching — save, restore, experiment freely
- One command deploys, ~25 second updates
- Upgrade path to Fargate + Aurora when you're ready

### What it costs

Dev mode runs on Lambda + CloudFront + SQLite-on-S3. Almost everything is free tier.

| Resource | Monthly |
|---|---|
| Lambda + CloudFront | $0.00 |
| DynamoDB (API keys) | $0.00 |
| S3 (database + snapshots) | $0.01 |
| Secrets Manager | $0.40 |
| **Total** | **$0.42** |

### Get started

```
git clone https://github.com/tokenburner-ai/stack
cd stack
tokenburner deploy
```

<p align="center">
<a href="https://tokenburner.ai">tokenburner.ai</a>
</p>

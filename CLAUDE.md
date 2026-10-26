# Uptime Monitor
Serverless uptime checker. A Lambda pings URLs on a schedule, stores
results in DynamoDB, and a React dashboard displays them.
## Stack
- infra/: Terraform, AWS provider, remote state in S3
- backend/: TypeScript Lambdas (Node 20), AWS SDK v3
- frontend/: Vite + React + TypeScript
## Rules
- Free tier only. Never propose EC2, RDS, NAT Gateway, or provisioned
capacity. Flag anything that could cost money.
- Never hardcode credentials or account IDs. Use env vars / IAM roles.
- Explain every change before making it. I am re-learning; teach as you go.
- Small commits. Run tests before saying something is done.
- If unsure about an AWS behaviour, say so instead of guessing.
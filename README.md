# Hey, I'm Brandon 👋🏾

I build serverless applications on AWS. Owner of [ur/gd Studios](https://urgdstudios.com) — a creative technology studio focused on calm, well-architected tools.

By day I'm a Senior Program Manager at Amazon, where I architect AI-driven decision systems and operational tooling. By night I design and ship production software on AWS — from concept through infrastructure-as-code to CI/CD pipeline.

Currently pursuing AWS Solutions Architect Associate (Cloud Practitioner certified).

---

## What I Build

### [Pulse](https://github.com/brandon-urgd/pulse) — AI-Guided Feedback Platform

Multi-tenant SaaS that turns documents into AI-guided feedback sessions. Upload content, share a link, reviewers have a structured conversation with an AI agent, and you get synthesized insights.

- 64 Lambda functions (Node.js 22), API Gateway (51 routes), Bedrock Claude
- 7 DynamoDB tables, S3 document storage, Cognito + session token dual auth
- Bedrock response streaming via Lambda Function URLs
- 9,400-line CloudFormation template, 3 environments, GitHub Actions CI/CD
- Stripe billing, EventBridge scheduling, X-Ray tracing, 9 CloudWatch alarms
- Semgrep + Checkov security scanning, WAF protection

### [Chronicle](https://github.com/brandon-urgd/chronicle) — Professional Narrative System

Native desktop app that captures daily work, organizes it under programs and goals, and generates leadership-ready reports. Built for program managers who need structured exports at review time.

- React 19 + TypeScript frontend, Rust backend (axum 0.7, tokio, rusqlite)
- Single-binary Tauri desktop app — sub-second startup, ~6 MB installer
- ~95 API routes, SQLite with WAL mode (21 tables), PDF export
- MCP server for AI-assisted reporting and weekly update generation

### [Stitch](https://github.com/brandon-urgd/stitch) — SVG to Embroidery Converter

Production web app that converts SVG files to PES embroidery format. Live at [stitch.urgdstudios.com](https://stitch.urgdstudios.com).

- Event-driven architecture: presigned URL upload → GuardDuty malware scan → Lambda conversion → status polling
- CloudFront + S3 hosting, API Gateway, DynamoDB status tracking
- Zero-touch security — infected files never reach application compute

### [urgdstudios.com](https://github.com/brandon-urgd/urgdstudios.com) — Studio Website

Company website with React 19 SSR pre-rendering, CloudFront + S3 hosting, Lambda contact form intake, and automated CI/CD.

---

## Tech I Work With

**Compute:** Lambda (Node.js 22, Python 3.13), Bedrock (Claude)  
**Storage:** DynamoDB, S3, SQLite  
**Networking:** CloudFront, API Gateway, Route 53  
**Auth:** Cognito, custom session tokens, API key auth  
**Security:** WAF, GuardDuty, Shield (malware scanning), Semgrep, Checkov  
**IaC:** CloudFormation (sole IaC — no Terraform, no CDK)  
**CI/CD:** GitHub Actions with OIDC, multi-environment promotion  
**Frontend:** React 19, TypeScript, Vite, CSS Modules  
**Desktop:** Tauri, Rust (axum, tokio, serde, rusqlite)  
**Monitoring:** CloudWatch (alarms, dashboards, metrics), X-Ray, SNS alerting  

---

## About ur/gd Studios

[urgdstudios.com](https://urgdstudios.com) · Seattle, WA

Every application follows the same principles: serverless-first, infrastructure-as-code, least-privilege IAM, multi-environment CI/CD, and security scanning before every deploy.

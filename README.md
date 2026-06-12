<div align="center">

# Srashti Gupta

**Full Stack Software Engineer · 5 years production engineering · MS CS @ Northeastern (4.0 GPA)**

[![Portfolio](https://img.shields.io/badge/Portfolio-srashtigupta--25.github.io-c8622a?style=flat-square&logo=safari&logoColor=white)](https://srashtigupta-25.github.io)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-srashti--gupta-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/srashti-gupta-07b634151)
[![Email](https://img.shields.io/badge/Email-sg.srashtigupta@gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:sg.srashtigupta@gmail.com)
[![Resume](https://img.shields.io/badge/Resume-Download-4CAF50?style=flat-square&logo=adobeacrobatreader&logoColor=white)](https://srashtigupta-25.github.io/resume.pdf)

**Open to 2026 SWE Internship · Available July-December 2026**

</div>

---

## What I Build

I build full stack systems that scale - distributed backend APIs handling millions of requests, AI-powered serverless pipelines on AWS, and React frontends. Over 5 years at **NAB, IBM, and Capgemini**, I've shipped production software for banking, enterprise, and global clients. Most recently I shipped **Sage** - a live AI research synthesizer on AWS Bedrock.

---

## Featured Project — Sage AI Research Synthesizer

> **Ask anything. Understand everything.** · [Try it Live →](https://d1kbvlvilht945.cloudfront.net)

A production-grade AI research platform that decomposes any topic into parallel research threads, grounds findings in real-time web data, and delivers a structured intelligence brief in **under 45 seconds** - built entirely on AWS serverless infrastructure.

```
POST /reports
     │
     ▼
API Gateway → Cognito JWT Auth → Lambda Orchestrator
     │
     ▼
Step Functions: SagePipeline
     │
     ├─ State 1: Decompose  (Claude Haiku 4.5) → 3 sub-questions
     │
     ├─ State 2: Research × 3  (Map state — true parallel)
     │           Tavily web search + Claude Haiku 4.5
     │
     ├─ State 3: Generate Report  → structured 350–900 word brief
     │
     └─ State 4/5: Images + Persist → DynamoDB (status: COMPLETE)

Frontend polls GET /reports/{id} every 3s until COMPLETE (~45s avg)
Deployed: S3 + CloudFront · Cognito auth · PDF export · Mobile responsive
```

| Service | Role |
|---|---|
| AWS Lambda (9 functions) | Serverless Java 25 handlers — zero server management |
| Step Functions | 5-state chain-of-thought pipeline with parallel Map execution |
| Amazon Bedrock | Claude Haiku 4.5 - decompose, research, synthesize |
| DynamoDB | Per-user report isolation, on-demand billing |
| CloudFront + S3 | Global CDN, HTTPS, sub-50ms load times worldwide |
| Cognito | User signup, email verification, JWT authorization |

**Stack:** `Java 25` `AWS Lambda` `Step Functions` `Amazon Bedrock` `DynamoDB` `CloudFront` `Cognito` `IAM` `React 18` `Tavily API`

---

## Other Projects

### [Adaptive Concurrent Web Server](https://github.com/cs5600-sp26/project-webserver-team0100)
Multi-threaded Rust web server with adaptive worker pool that dynamically scales thread count based on real-time request load — using only Rust stdlib (no Tokio, no Rayon).

**Result:** P99 latency cut from **1.73ms → 1.04ms** (40% reduction) at **31,725 req/s**

`Rust` `Python` `Shell Scripting` `OS-level concurrency` `Systems Programming`

### [Streaming Analytics Data Warehouse](https://github.com/srashtigupta-25/Streaming-Analytics-Data-Warehouse)
Year-partitioned star schema in cloud-hosted MySQL with a Dockerized R-based ETL pipeline - processes 98K+ streaming transaction records across 3+ years of viewership data.

`R` `MySQL` `Docker` `ETL` `Star Schema` `Data Engineering`

---

## Experience

| Company | Role | Impact |
|---|---|---|
| **NAB Global Innovation Center** | Senior Software Engineer · Feb 2023–Jul 2025 | 35% API latency reduction · 1M+ daily requests · STAR + SPOT Awards |
| **IBM India** | Software Engineer · Apr 2021–Dec 2022 | 45% system performance improvement · 40% faster CI/CD releases |
| **Capgemini Engineering** | Software Engineer · Jan 2019–Mar 2021 | 14 microservices · Samsung + Hughes.net · Team Excellence Award |

---

## Tech Stack

```
Languages      Java · Python · Rust · C++ · JavaScript · Node.js · SQL · R · Shell Scripting
Backend        Spring Boot · Spring Data JPA · Hibernate · Microservices · RESTful APIs · React
Databases      DynamoDB · PostgreSQL · MySQL · MongoDB · Redis · Oracle
Cloud          AWS (Lambda · Bedrock · Step Functions · CloudFront · Cognito · IAM · SQS · SNS · EC2 · S3 · RDS)
DevOps         Docker · Kubernetes · CI/CD · Linux · Maven · Gradle
Messaging      Apache Kafka · Step Functions · Swagger/OpenAPI
Concepts       Generative AI · Prompt Engineering · Serverless · System Design · Event-Driven Architecture · TDD
```

---

## Education

| Degree | School | GPA |
|---|---|---|
| MS, Computer Science | Northeastern University, Boston MA · Expected May 2027 | **4.0** |
| BTech, Information Technology | Banasthali Vidyapith, India · May 2019 | **3.7** |

---

<div align="center">

![GitHub Activity](https://ghchart.rshah.org/c8622a/srashtigupta-25)

**Open to 2026 SWE internship opportunities in the US · Available July–December 2026**

[Portfolio](https://srashtigupta-25.github.io) · [LinkedIn](https://linkedin.com/in/srashti-gupta-07b634151) · [sg.srashtigupta@gmail.com](mailto:sg.srashtigupta@gmail.com)

</div>

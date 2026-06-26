<div align="center">

# Hi, I'm Srashti Gupta

### Production software engineer building AI-powered systems

**5+ years of engineering experience · MS Computer Science @ Northeastern University · 4.0 GPA**

[![Portfolio](https://img.shields.io/badge/Portfolio-Explore_my_work-2459D3?style=for-the-badge&logo=safari&logoColor=white)](https://srashtigupta-25.github.io)
[![Résumé](https://img.shields.io/badge/Résumé-View-13203A?style=for-the-badge&logo=readthedocs&logoColor=white)](https://srashtigupta-25.github.io/resume.pdf)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/srashti-gupta-07b634151)
[![Email](https://img.shields.io/badge/Email-Say_hello-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:sg.srashtigupta@gmail.com)

**Open to software engineering internship opportunities in the US**

</div>

---

## What I bring

My background is in production backend and distributed systems engineering. I spent more than five years building banking and enterprise software at **NAB, IBM, and Capgemini** before starting my master's at Northeastern.

Now I am applying that foundation to LLM workflows, multi-agent systems, and serverless AI products. I care about the parts that turn a promising prototype into dependable software: API design, latency, failure handling, testing, deployment, and observability.

| Production engineering | AI systems | Measured impact |
|---|---|---|
| Java, Spring Boot, AWS, microservices | Python, LangChain, LangGraph, LLM APIs | **35%** lower API latency |
| Distributed and event-driven systems | Multi-agent orchestration, Bedrock, Claude | **1M+** requests handled daily |
| Docker, Kubernetes, Kafka, CI/CD | Grounded web research and tool-calling agents | **3** industry awards |

---

## Featured AI systems

### [Sage Research Synthesizer](https://d1kbvlvilht945.cloudfront.net)

**A serverless LLM research system built in Java and AWS.**

Sage decomposes a topic into three research paths, grounds each path in live web data, runs the work in parallel through Amazon Bedrock, and returns a structured brief in under **45 seconds**.

```text
Question
   │
   ▼
API Gateway → Cognito → Java Lambda
   │
   ▼
AWS Step Functions
   ├── Decompose with Claude
   ├── Research × 3 in parallel
   │     └── Tavily web search + Claude on Bedrock
   ├── Generate structured report
   └── Persist to DynamoDB
```

- Cut research time by roughly **60%** compared with the sequential workflow
- Built a five-state Step Functions pipeline with retry and execution visibility
- Used nine Java 25 Lambda functions across orchestration, research, persistence, and retrieval
- Added Cognito JWT authentication, PDF export, and CloudFront delivery

**Stack:** `Java 25` `Amazon Bedrock` `Claude` `AWS Lambda` `Step Functions` `Tavily` `DynamoDB` `Cognito` `React`

[Live demo →](https://d1kbvlvilht945.cloudfront.net) · [Repository →](https://github.com/srashtigupta-25/sage-research-synthesizer)

---

### [Alpha Sign](https://alpha-sign-zeta.vercel.app)

**A team-built, multi-agent financial intelligence platform.**

Alpha Sign coordinates four specialist agents to turn a ticker into narrative research, quantitative signals, regime analysis, and an executive report.

I owned the **Narrative/News Agent** workflow and co-developed the **LangChain/LangGraph** agent layer with a teammate. My work covered ticker-aware news research, source reliability, multi-ticker support, narrative synthesis, and orchestration safeguards.

```text
Narrative / News Agent
          │
          ▼
Signal Processing Agent → Latent State Agent
          │                       │
          └──────────┬────────────┘
                     ▼
              Executive Report
```

- Built an LLM-assisted news pipeline with source-quality checks and ticker filtering
- Added structured agent messaging and live activity streaming through Server-Sent Events
- Helped implement tool-calling workflows using LangChain and LangGraph
- Supported market analysis, Kalman-style regime detection, and PDF report generation

**Stack:** `Python` `LangChain` `LangGraph` `LLM APIs` `Next.js` `TypeScript` `SSE` `Docker`

[Live demo →](https://alpha-sign-zeta.vercel.app) · [Team repository →](https://github.com/Dankguy17/AlphaSign) · [My commits →](https://github.com/Dankguy17/AlphaSign/commits/main/?author=srashtigupta-25)

---

### [Autopsy Lab](https://autopsy-lab.vercel.app)

**An AI incident reconstruction engine built in four hours at the Madison AI Hackathon.**

Autopsy Lab converts raw system logs into an evidence-backed incident timeline, severity assessment, likely root cause, and prioritized remediation plan. After the hackathon, I hardened the prototype for public review with safer file processing, schema-validated LLM output, automated tests, CI, and a responsive interface.

- Built the analysis API with FastAPI, Groq, Llama 3.3, and Pydantic
- Added in-memory parsing for TXT, LOG, PDF, and DOCX files with size and type validation
- Shipped a Next.js and TypeScript interface with sample mode and JSON report export
- Added pytest, Playwright, GitHub Actions, Docker, and a unified Vercel deployment

**Stack:** `Python` `FastAPI` `Groq` `Llama 3.3` `Pydantic` `Next.js` `TypeScript` `Playwright`

[Live demo →](https://autopsy-lab.vercel.app) · [Repository →](https://github.com/srashtigupta-25/hackathon-1)

---

## Systems and data projects

### Adaptive Concurrent Web Server

Built a multithreaded Rust server with an adaptive worker pool that scales with real-time request load.

**Result:** Reduced P99 latency from **1.73 ms to 1.04 ms**, a 40% improvement at **31,725 requests/second**.

`Rust` `Python` `Concurrency` `Load testing` `Systems programming`

[Team repository →](https://github.com/cs5600-sp26/project-webserver-team0100) · [Read the case study →](https://srashtigupta-25.github.io/StreetLegal-Webserver-presentation.pdf)

### [Streaming Analytics Data Warehouse](https://github.com/srashtigupta-25/Streaming-Analytics-Data-Warehouse)

Built a Dockerized R ETL pipeline and year-partitioned MySQL star schema for **98,472 streaming transaction records** across more than three years of viewership data.

- Modeled 13 dimensions and one fact table for analytical querying
- Built a reproducible Dockerized ETL workflow in R and MySQL
- Surfaced a **34% Q4 2023 viewership increase** over Q4 2022

`R` `MySQL` `Docker` `ETL` `Star schema` `Data modeling`

[Repository →](https://github.com/srashtigupta-25/Streaming-Analytics-Data-Warehouse)

---

## Production experience

| Company | Role | Engineering impact |
|---|---|---|
| **NAB Global Innovation Center** | Senior Software Engineer | Reduced API latency **35%** across 20+ services handling **1M+ daily requests**; migrated 20 banking microservices to Java 17; earned STAR and SPOT Awards |
| **IBM India** | Software Engineer | Improved system performance **45%** with resilient microservice patterns; cut release cycles **40%** through Jenkins and Docker automation |
| **Capgemini Engineering** | Software Engineer | Reduced response time **25%** across 14 microservices; achieved **98%** automated test coverage; earned Team Excellence Award |

---

## Technical toolkit

| Area | Technologies |
|---|---|
| **AI & LLM engineering** | LangChain, LangGraph, Amazon Bedrock, Claude, LLM APIs, multi-agent orchestration, prompt engineering |
| **Languages** | Java, Python, Rust, JavaScript, TypeScript, SQL, C++, R |
| **Backend** | Spring Boot, REST APIs, Microservices, Spring Data JPA, Hibernate, FastAPI, Node.js |
| **Cloud & platform** | AWS, Lambda, Step Functions, Docker, Kubernetes, Kafka, CI/CD, Linux |
| **Data systems** | PostgreSQL, MySQL, MongoDB, Redis, DynamoDB, Oracle |
| **Engineering** | Distributed systems, event-driven architecture, system design, TDD, performance engineering |

---

## Education

- **MS in Computer Science**, Northeastern University, GPA: **4.0**, expected May 2027
- **BTech in Information Technology**, Banasthali Vidyapith, GPA: **3.7**

---

<div align="center">

I am interested in teams building backend platforms, cloud products, developer infrastructure, or production AI systems.

[Portfolio](https://srashtigupta-25.github.io) · [Résumé](https://srashtigupta-25.github.io/resume.pdf) · [LinkedIn](https://linkedin.com/in/srashti-gupta-07b634151) · [Email](mailto:sg.srashtigupta@gmail.com)

</div>

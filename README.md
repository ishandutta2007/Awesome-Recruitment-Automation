# Awesome-Recruitment-Automation

# Top Recruitment Automation Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on AI Sourcing, Candidate Matching & Hiring Workflow Automation*  
**Last updated: October 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Recruitment Automation**. These tools enable talent acquisition teams to automate sourcing, resume screening, candidate matching, interview scheduling, and outreach—reducing time-to-hire while improving candidate quality and recruiter productivity.

**Examples** include Workday Connected Recruiting, Phenom, Eightfold.ai, Paradox, Gem, Fetcher, Beamery, Sense, HireEZ, and SeekOut (the category leaders).

**Open-source emphasis**: Recruitment Automation is a domain where open-source tooling is **emerging rapidly but remains fragmented**. The strongest active projects are **TalentFlow AI** and **HR-OS** for AI-native hiring pipelines, **TalentGraph AI** for semantic candidate search, and **OpenCATS** as the longest-standing traditional ATS. Most projects focus on specific slices—resume screening, semantic search, or interview automation—rather than full end-to-end recruitment automation. Organizations seeking complete enterprise automation should evaluate commercial platforms or plan for integration across multiple open-source components.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Workday Connected Recruiting](https://www.workday.com/)**  
  Talent acquisition within Workday's HCM suite with AI-assisted sourcing, candidate matching, automated scheduling, and connected workflows across recruiting, onboarding, and workforce planning.

- **[Phenom](https://www.phenom.com/)**  
  Talent experience management platform with AI-powered career site personalization, candidate matching, and recruitment marketing automation.

- **[Eightfold.ai](https://eightfold.ai/)**  
  Talent intelligence platform using deep learning for candidate matching, skills inference, and talent pipeline automation across sourcing and internal mobility.

- **[Paradox](https://www.paradox.ai/)**  
  Conversational AI recruiting assistant (Olivia) for automated screening, interview scheduling, and candidate communication via chat.

- **[Gem](https://www.gem.com/)**  
  Recruiting operations platform with talent CRM, automated outreach sequences, and pipeline analytics for sourcing teams.

- **[Fetcher](https://fetcher.ai/)**  
  Automated sourcing platform that finds and engages passive candidates via email with AI-personalized outreach.

- **[Beamery](https://beamery.com/)**  
  Talent lifecycle management platform with CRM, sourcing automation, and skills-based talent intelligence.

- **[Sense](https://www.sensehq.com/)**  
  Talent engagement platform with AI chatbots for candidate communication, automated scheduling, and recruitment marketing.

- **[HireEZ](https://hireez.com/)**  
  AI sourcing platform with candidate discovery, automated outreach, and talent pool management across multiple channels.

- **[SeekOut](https://seekout.com/)**  
  AI-powered talent search and analytics platform with diversity sourcing and candidate rediscovery capabilities.

## Open-Source GitHub Projects

- **[TalentFlow AI](https://github.com/Nihal-MN/talentflow-ai)**  
  Open-source AI-native hiring pipeline (AGPL-3.0) with structured talent data, explainable candidate matching, semantic search, and recruiter-in-the-loop workflows; self-hosted with Docker (PostgreSQL + pgvector), runs in **deterministic demo mode without API keys**, and includes synthetic seed data for testing; supports OpenAI integration for live extraction and screening; badges distinguish mock vs live extraction so behavior is never ambiguous .

- **[HR-OS](https://github.com/rathishreya/hr-os)**  
  Open-source AI-native hiring operating system (FastAPI + React) with core hiring loop, pluggable AI (Claude/Ollama/rule-based fallback), real SMTP email engine, and **MCP server exposing 10 hiring tools** for AI agent integration; runs locally with zero keys, upgrades to full AI when credentials are added; features AI screening interviews, human-overridable scoring, and audit trails .

- **[TalentGraph AI](https://github.com/Nihal-MN/talentgraph-ai)**  
  Open-source semantic talent search and rediscovery engine with hybrid retrieval (PostgreSQL FTS + pgvector), Reciprocal Rank Fusion, and **explainable ranking with source quotes**; parses natural-language queries ("senior Python backend engineer in Berlin with Kubernetes") and explains why each result matched; includes a measured benchmark with Precision@K, Recall@K, MRR, and nDCG; runs keyless in demo mode with 200 synthetic profiles .

- **[OpenCATS](https://github.com/opencats/OpenCATS)**  
  The longest-standing open-source ATS (MPL 2.0, ~757 GitHub stars, first code from 2007 CATS project); built for recruiters and agencies with pipeline management, career portals, and resume parsing; actively maintained with v0.11.1 released September 2026; **caution**: legacy codebase with 12 security advisories in 2026 (two critical) fixed in v0.10.0–v0.11.1—operators must track and install security updates promptly .

- **[Niyam](https://github.com/imrohit4077/niyam)**  
  AI-powered applicant tracking system positioned as a modern alternative to Greenhouse, Lever, and SmartRecruiters; FastAPI backend with React 19 frontend, PostgreSQL, Celery/Redis for async processing, JWT auth, and optional MinIO/S3 for file storage; includes audit logging, rate limiting, and Docker deployment .

- **[SmartRecruiter](https://github.com/aniGenAI/smartrecruiter)**  
  Skill-routed multi-agent architecture for resume screening and adaptive technical interviewing (research implementation); combines LLMs, semantic embeddings, and dynamic evaluator orchestration; supports resume PDF ingestion, semantic skill extraction, candidate vector storage (Qdrant), explainable evaluation reasoning, and recruiter-facing dashboard; Python/FastAPI with Ollama and React .

- **[OpenHire](https://github.com/DevSidd2006/OpenHire)**  
  AI-powered interview and candidate screening platform for high-volume hiring (campus recruitment focus); features structured voice interviews via Gemini Live, resume parsing, and **12 specialized LLM agents** for technical/behavioral evaluation, resume auditing, integrity checking, and bias detection; runs offline in mock mode without API keys; 911 automated tests included .

### Additional Strong Open-Source Options

- **Horilla** — Open-source HRMS with recruitment module covering job postings, applicant tracking, drag-and-drop pipeline stages, and interview scheduling; Django/PostgreSQL stack with Docker support; LGPL-2.1 licensed and actively released (v2.1.8, September 2026) .
- **Frappe HR** — Open-source HR and payroll suite with job opening, applicant, and interview records; GPL-3.0 licensed with frequent releases (v16.20.0, September 2026); best suited for organizations already using the Frappe/ERPNext ecosystem .
- **OrangeHRM Community** — GPL-3.0 HR suite with basic recruitment module (job postings, applicant tracking, interview scheduling); cleaner UI than OpenCATS but recruiting handles internal HR workflows better than external agency needs .
- **SpotAxis** — MIT-licensed ATS with career sites, resume parsing, and custom pipelines per job; supports multi-company hosting mode; **caution**: 31 GitHub stars, no releases, last commit October 2025—check activity before adopting .

**Frameworks for building custom systems**: Combine **TalentFlow AI** for an AI-native hiring pipeline with explainable matching, **TalentGraph AI** for semantic talent search and rediscovery, **HR-OS** for MCP-driven agent automation with real email outreach, and **OpenCATS** as a traditional ATS foundation if full pipeline management is needed in a self-hosted recruitment automation stack; layer **OpenHire** for AI-driven voice screening in high-volume scenarios.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Recruitment automation platforms handling candidate data must comply with applicable employment laws, anti-discrimination regulations, and data privacy requirements (GDPR, CCPA); AI-driven screening requires bias auditing and human oversight.
- **Open-source recruitment automation is emerging but fragmented**—TalentFlow AI and HR-OS provide strong AI-native pipelines, TalentGraph AI excels at semantic search, but no single open-source platform covers the full enterprise automation lifecycle (sourcing → screening → scheduling → offer → onboarding) with the depth of Phenom or Eightfold. OpenCATS is mature but carries legacy security debt. Organizations requiring complete automation should plan for commercial platforms or integration across multiple open-source components.
- Verify license terms for commercial use; TalentFlow AI uses AGPL-3.0 , OpenCATS uses MPL 2.0 , Horilla uses LGPL-2.1 , and Frappe HR uses GPL-3.0 .

---

**Made for talent acquisition leaders, recruiting operations teams, HR technologists, and sourcing specialists.**  
Let's make recruitment automation more open, explainable, and candidate-respectful.

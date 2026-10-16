# Félix Lezama — Data, Automation & Applied AI

**Data Analyst · BI Developer · AI Workflow & Data Automation** — Python, SQL, Power BI, n8n, LLM integrations. Based in Buenos Aires, Argentina · open to 100% remote roles across the Americas.

I came to data from the field. After years running electronic security operations — CCTV, access control, monitoring centers, B2B contracts — I moved into data analytics and automation. Today I build data pipelines, dashboards and small production systems for a real industrial client and for my own products, under my independent brand **TechCam**. I'm also studying for a degree in Data Science & AI (IFTS N.º 18).

I build with AI coding agents (Claude Code) using spec-driven development: written specs, test-first, documented decisions. I design, review and operate everything I ship.

## What I'm looking for

Remote roles as **Data Analyst / BI Developer / Analytics Engineer** or **AI Workflow & Data Automation Engineer** — full time or B2B contractor.

## Selected work

| Project | Problem | What I built | Result |
|---|---|---|---|
| **Fleet repair log with AI receipt reading** (industrial client) — [case study](https://github.com/Darkslidex/fleet-receipt-reader-case-study) | Repair costs were typed by hand into a years-old spreadsheet that depended on one person | Web app that reads repair receipts from a phone photo with a multimodal LLM, FastAPI + PostgreSQL, daily backups with tested restore | In production · my most complex system: AI reads supplier 97% and amount 90% vs. 27% and 3% for OCR, 9 services, 2,300+ automated tests, planning to production in 3 days |
| **Supply chain data pipeline & dashboard** (industrial client) | Foreign-trade data arrived as scattered email reports | Python + n8n pipeline into PostgreSQL, star schema with DAX measures, Power BI dashboard | In production · 15 data-quality validations, 3-layer alerting, dead-man switch, 84 s end to end, incidents documented with root cause |
| **Stock lookup without SAP** (industrial client) | Checking stock required a dedicated PC with SAP installed | Web app that queries ERP stock directly (FastAPI, HTMX) | Pilot deployed |
| **SQL Trainer** — [sql.techcam.com.ar](https://sql.techcam.com.ar) | Getting interview-ready in SQL for data roles | PWA running real SQL in the browser (sql.js/WebAssembly), deterministic grading, AI tutor behind a FastAPI proxy with Argon2id and rate limits | In production · mutation-tested, 200+ documented decisions |
| **Python Trainer** | Practicing Python with no server and no constant connection | Python in the browser (Pyodide in an isolated Web Worker), 14-concept curriculum, deterministic exam, installable offline PWA | In production · 91/91 functional and 17/17 non-functional requirements passing |
| **AI nutrition assistant** (personal) | Logging meals and macros had too much friction | Telegram bot: one sentence → calories and macros via an LLM, guarded by deterministic validation and a fallback model; PWA dashboard behind Cloudflare Access | In daily use · 1,300+ tests · disabling model reasoning cut response time from 18.8 s to 9.6 s |

Client systems are shown without names or business figures, and their code is private.

## Start here

- [**fleet-receipt-reader-case-study**](https://github.com/Darkslidex/fleet-receipt-reader-case-study) — my flagship project: phone photo → isolated AI reader → human confirmation → clean data in Excel and KPIs. Architecture, security decisions and measured results (client code stays private).
- [**pipeline-bi-calidad-datos**](https://github.com/Darkslidex/pipeline-bi-calidad-datos) — BI pipeline with a column contract, row-level Pydantic quarantine, star schema and a 12-rule DAMA data-quality audit (synthetic data, runnable).

## Also built

- **Daily work organizer** — offline-first PWA with an AI coach and a finance module with an append-only audit log and inflation adjustment.
- **B2B prospecting agent** — Claude Code with two custom MCP servers, deterministic scoring and human approval of every email via Telegram (archived).
- **Multi-vertical CRM** — Next.js, TypeScript, Prisma and PostgreSQL with map views, plus an LLM contact-enrichment pipeline (decommissioned).
- **Rental catalog backend** for a client — FastAPI with one test per business rule, Cloudflare Access, encryption at rest.
- **Landing page network** — portal plus audience-specific sites with strict CSP and a lead backend (Fastify, PostgreSQL, AES-256).
- **Early computer-vision prototypes** — [DeepVision](https://github.com/Darkslidex/DeepVision) (operator monitoring with YOLO + pose) and [sentinel-ai](https://github.com/Darkslidex/sentinel-ai) (perimeter detection + fraud classifier demo). Unfinished; kept public as learning projects.
- **Claude Code skills & security hooks library** — DAMA data-quality audits, a read-only supervisor and a PreToolUse security hook, synced across three environments.
- **Generative AI video** — directed Ana, a consistent digital character, across 30 short videos (130+ clips with Google Veo and Gemini Omni), edited and adapted for TikTok and Meta Ads, with a documented prompt method for character and camera continuity.

## Stack

**Data:** Python (pandas, Pydantic), SQL (PostgreSQL, SQLite, MySQL), Power BI (DAX, Power Query), DAMA-DMBOK data quality
**Automation & AI:** n8n, LLM APIs via OpenRouter, Claude Code, MCP servers
**Backend & web:** FastAPI, SQLAlchemy, Alembic, PWA (Service Worker, IndexedDB), HTMX
**Quality & ops:** pytest, Hypothesis, mutation testing, Playwright · Docker, Coolify, Linux, Cloudflare (Tunnel, Access) · gitleaks, pip-audit, Trivy

## Contact

[LinkedIn](https://linkedin.com/in/felix-lezama/) · [Online CV](https://micv.techcam.com.ar)

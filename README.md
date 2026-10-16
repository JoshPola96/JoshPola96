# Hi 👋, I'm Joshua Peter Polaprayil

**AI/ML Engineer · MSc Big Data Analytics & AI · Kottayam, Kerala, India — available now, open to remote worldwide**

I build AI systems that survive contact with production: the model, the API around it, the infrastructure under it, and the monitoring that tells you when it breaks.

📧 [josh19peter96@gmail.com](mailto:josh19peter96@gmail.com) · 💼 [LinkedIn](https://www.linkedin.com/in/josh33-peter10/)

---

## 🧭 How to read this profile

Every repository here is labelled with its origin, because context changes what the code is telling you:

| Label | What it means |
|---|---|
| **Production case study** | A system that ran live with real users. Architecture and trade-offs documented; source is proprietary. |
| **Certification capstone** | Peer-reviewed submission assessed against a published rubric — DataTalksClub Zoomcamps, Coursera specializations. |
| **Timeboxed assessment** | A technical take-home, 3 hours to 5 days. Each carries a *Scope & trade-offs* section: what was in scope, what I cut, and what I'd change with more time. |
| **Internship coursework** | Work from my Data Science & ML internship at Irohub Infotech (2024–25), published here after it ended. |
| **Academic** | MSc coursework and dissertation artifacts, published as-is. |
| **Personal project** | Built on my own time. Complete rather than tended, unless it says otherwise. |

### These are dated artifacts, not maintained software

Every repository states the year it was built. Most were written between 2021 and 2025, against the libraries of that moment, with unpinned dependencies.

Python's ML ecosystem does not hold still. Since then pandas, numpy, PyTorch, Airflow and MLflow have all shipped breaking major versions. A repository last worked on in 2025 that no longer installs cleanly in 2026 is behaving exactly the way an unmaintained repository behaves. **That is a fact about the calendar, not a finding about the engineering.**

Two have since been rebuilt properly — dependencies pinned to a lockfile, notebooks re-run from a clean kernel, every reported number traceable to its own output. The rest have not. I am working through them, and that is what the finished ones look like.

Where a build is currently failing, I've said so in that repository's README — along with the specific cause, the specific line, and the fix. Nothing is hidden behind a green badge.

### None of this is commercial software

No revenue depends on any of it. No users are supported, no SLA exists, and nobody is paying for it to keep running. These are assessments, capstones, coursework and personal builds, published so the work is inspectable.

Two systems I worked on *were* live and commercial — the **Esimtime** agent platform and the **Hubinit** loyalty platform, which reached live deployment before the company wound down. Their code belongs to those companies. What is published here is the architecture and the product reasoning behind each: the [Esimtime case study](https://github.com/JoshPola96/enterprise-ai-agent-architecture-esim) and the [loyalty platform case study](https://github.com/JoshPola96/loyalty-platform-product-case-study). Neither is source, and neither is a running system.

### What these repositories can actually tell you

How a problem was scoped. What was cut, and why. Whether the trade-off can be articulated afterwards. That is what each README documents, and it's the part that doesn't expire.

If you want to see how I write code today, look at what carries a current date. Older repositories show where I was, not where I am — which is true of everyone's.

I'm glad to bring any of this current if it's genuinely useful to you. Ask, and I will.

---

## 🚀 Most recent role

**Full-Stack AI Engineer — Esimtime** *(Jul 2025 – Jul 2026 · remote, US)* — **now concluded; open to new work**

Sole architect of a conversational commerce platform running the full eSIM lifecycle on WhatsApp and Telegram.

* Stateful **LangGraph** agent over **26 schema-validated tools**, >99% tool execution accuracy
* Hybrid **Qdrant** retrieval — server-side dense + sparse fusion with cross-encoder reranking, 15–25% relevance lift over single-method search
* Self-hosted speech (**faster-whisper**, **Piper**) — no per-minute billing, models chosen by measured latency/memory benchmarks
* Ten-layer security architecture built after a live exploitation attempt; held **300+ RPS** adversarial load with 100% legitimate-traffic success
* Ranked **Top 5 AI company on F6S** (May 2026) and Top 5 of 39 at an investor showcase

👉 **[Read the architecture case study](https://github.com/JoshPola96/enterprise-ai-agent-architecture-esim)**

---

## 🔨 Recent and next

**[ai-data-agent](https://github.com/JoshPola96/ai-data-agent)** — a data analyst you can hand the exports you actually have. Ask in any language: it reads PDFs, Word files and spreadsheets, computes the statistics itself instead of guessing them, and answers with a chart, a multi-panel dashboard or a flowchart built from a document's prose. It also **profiles every table for the flaws that silently corrupt an aggregate** — a `TOTAL` row loaded as data, four spellings of one region, the same measure present twice in different currencies — and names them beside the figure they affect. Every number traces to the tool that produced it; arithmetic in prose is forbidden, because a number a model produced in its own head is a number nobody can check. ReAct loop, no framework underneath, 558 offline tests. Complete.

**[HateAtlas](https://huggingface.co/datasets/JoshPola96/HateAtlas)** *(October 2026)* — 21 published English hate-speech datasets read onto one schema, with each text's hate level, the groups it targets, and every source's own label, id and author kept beside it. Published in three configurations because share-alike and non-commercial licences cannot share a table. It exists because my 2021 dissertation concluded the field needed better data and I finally went and built it: racism becomes a filter across sources, platforms and authors instead of one dataset's nine. Citable by DOI, [10.57967/hf/10899](https://doi.org/10.57967/hf/10899).

**Notebook 2** — in progress, slowly. Current methods on HateAtlas: BERT fine-tuned inside the hybrid, further pretraining on the task's own text, functional tests beyond a random split, and bias measured across groups.

**The Children of Sodom (CrewAI)** — paused while the rebuilds take priority. A study and simulation of how ordinary people become cruel together: how a grievance is assembled by a crowd, hardens into something with a will of its own, and consumes the people who built it. Its agents are grounded in the social psychology of evil — Bandura on moral disengagement, Asch on conformity, Haslam on dehumanisation, Girard on scapegoating, with Milgram, Zimbardo, Staub and Reicher behind them — then run to find which mechanisms the behaviour actually requires and which it can do without.

Built to be falsifiable rather than merely interesting: four independent coders against one codebook, ablations with family-wise corrected intervals, null, held-out and sensitivity tests, a stated minimum detectable effect, and 34 structural invariants checked on every run. Its one finding — that moral disengagement carries the model — survives all four coders at +42.5 to +43.9. A hobbyist project, not formal research: no institutional review, and the underlying account is private.

---

## 📌 Selected work

| Project | What it does | Stack |
|---|---|---|
| **[dissertation-racism-detection-bert-cnn-bilstm](https://github.com/JoshPola96/dissertation-racism-detection-bert-cnn-bilstm)** | Tells racist tweets from the rest: BERT-large read by CNN and BiLSTM layers, plus a hybrid that adds each tweet's sentiment and style. The 2021 submission is kept unchanged beside the rebuilt, runnable version, and the repository is home to **HateAtlas** | TensorFlow · BERT-large · uv |
| **[ai-data-agent](https://github.com/JoshPola96/ai-data-agent)** | Answers questions about your PDFs, Word files and spreadsheets in any language, computes the statistics itself, and returns charts, dashboards and flowcharts beside the answer — every figure traceable to the tool that produced it | FastAPI · FAISS · Redis · OpenAI/Gemini |
| **[company-bankruptcy-prediction-mlops](https://github.com/JoshPola96/company-bankruptcy-prediction-mlops)** | Predicts which companies are heading for bankruptcy from their financial statements, then watches its own accuracy and retrains itself when the incoming data drifts. Ingestion, training, evaluation, promotion and deployment are orchestrated end to end, with no manual step | Airflow · MLflow · Terraform · AWS |
| **[heart-attack-data-pipeline](https://github.com/JoshPola96/heart-attack-data-pipeline)** | Turns a raw heart-attack risk dataset into a queryable warehouse and a Power BI dashboard — infrastructure, ingestion, transformation and charts, none of it done by hand | GCP · dbt · BigQuery · Airflow |
| **[rppg-monitor](https://github.com/JoshPola96/rppg-monitor)** | Reads heart rate, HRV and respiration from an ordinary webcam — no contact, no wearable — streamed live to the browser. A five-day take-home built on the research rPPG library of [wiseai.care](https://www.wiseai.care/), founded by MIT graduates: theirs needs direct camera access, so this re-does capture over WebSockets, holding accuracy within 1–3 BPM on 37 MB instead of 552 MB | MediaPipe · OpenCV · FastAPI |
| **[gloved-ungloved-yolov8](https://github.com/JoshPola96/gloved-ungloved-yolov8)** | Detects whether the hands in an image are gloved, for PPE compliance — with CLIP and pose estimation cross-checking every label before a single epoch runs | YOLOv8 · CLIP · Streamlit |

---

## 🧰 Tech stack

**AI / ML** Python · PyTorch · TensorFlow · scikit-learn · Transformers (BERT, BioBERT) · LangChain · LangGraph · RAG · NLP · YOLOv8 · OpenCV · OCR

**MLOps** Apache Airflow · MLflow · dbt · Evidently AI · Docker · Terraform · GitHub Actions · Model monitoring · Retraining pipelines

**Backend** FastAPI · Flask · NestJS · .NET Core · REST APIs · JWT auth · SQLAlchemy · Prisma

**Data** PostgreSQL · SQL Server · Redis · BigQuery · Qdrant · FAISS · ChromaDB · Pandas · NumPy · PySpark · Databricks

**Cloud** AWS (EC2, S3, RDS, Lambda) · GCP (BigQuery, GCS) · Nginx · Linux

**Frontend** Streamlit · React · TypeScript · HTML/CSS · Bootstrap

---

## 🎓 Certifications

Externally assessed, peer-reviewed against published rubrics:

* **[MLOps Zoomcamp](https://certificate.datatalks.club/mlops-zoomcamp/2025/c8e8b5ba3fbcfde9632b6c623269ae4bbde4a2d2.pdf)** — DataTalksClub, Aug 2025
* **[Data Engineering Zoomcamp](https://certificate.datatalks.club/dezoomcamp/2025/c8e8b5ba3fbcfde9632b6c623269ae4bbde4a2d2.pdf)** — DataTalksClub, Apr 2025
* **[dbt Fundamentals](https://credentials.getdbt.com/38b4d310-089d-4261-9ac6-9487f2f820dc)** — dbt Labs, Feb 2025
* **[Web Design for Everybody](https://www.coursera.org/account/accomplishments/specialization/certificate/F2JC63D3GSUT)** — University of Michigan / Coursera, Sep 2023

---

## ✍️ Writing

**[The Architecture of Trust: What a Cyberattacking AI and a Grafana Experiment Taught Me About Governance](https://www.linkedin.com/pulse/architecture-trust-what-cyberattacking-ai-grafana-me-joshua-l8tjc/)** — written after a real exploitation attempt against the production agent I built, on what it changed about where I put trust boundaries and how I think about governance.

---

## 🛠️ Background

Around four years across database engineering (SQL Server and ETL for US real-estate firms at Datafloat), enterprise .NET (owned a loan-assessment application's move from Excel/VBA to C#/.NET at Permanent TSB, Dublin, through its first release), early-stage product and backend (defined the domain and MVP for a loyalty platform at Hubinit, then owned the NestJS/PostgreSQL/AWS backend after the lead left, and led the response to a bot attack), and computer vision (YOLOv7 for vehicle-light and crosswalk detection in ADAS at RoshAI).

Between the Dublin role and the return to tech I worked full-time in Ireland across Dublin Airport airside logistics, bonded warehousing and HACCP-regulated manufacturing, on 12-hour rotating night shifts, self-funding relocation and retraining. Airside access meant Garda vetting, a blue badge, and EU aviation Basic Security Awareness Training under EU 300/2008 — insider threat, radicalisation, security culture and cybersecurity — alongside HACCP and manual handling certification. That's on the CV deliberately: it's where the execution discipline came from, and the habit of delivering every shift.

Also holds PG diplomas in Airport Cargo Management and Logistics & Supply Chain Management, which is how the eSIM-commerce domain stopped being unfamiliar territory.

**Languages** Malayalam (native) · English (fluent) · Hindi, Tamil, German (beginner)

---

⭐ Open to full-time, contract and freelance work. Happy to talk architecture, tradeoffs, or anything in the repos above — [get in touch](mailto:josh19peter96@gmail.com).

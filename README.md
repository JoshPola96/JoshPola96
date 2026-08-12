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
| **Academic** | MSc coursework and dissertation artifacts, published as-is. |
| **Personal project** | Built on my own time. Complete rather than tended, unless it says otherwise. |

### These are dated artifacts, not maintained software

Every repository states the year it was built. Most were written between 2021 and 2025, against the libraries of that moment, with unpinned dependencies.

Python's ML ecosystem does not hold still. Since then pandas, numpy, PyTorch, Airflow and MLflow have all shipped breaking major versions. A repository last worked on in 2025 that no longer installs cleanly in 2026 is behaving exactly the way an unmaintained repository behaves. **That is a fact about the calendar, not a finding about the engineering.**

Where a build is currently failing, I've said so in that repository's README — along with the specific cause, the specific line, and the fix. Nothing is hidden behind a green badge.

### None of this is commercial software

No revenue depends on any of it. No users are supported, no SLA exists, and nobody is paying for it to keep running. These are assessments, capstones, coursework and personal builds, published so the work is inspectable. The Esimtime platform *was* live and commercial, but what is published here is an architecture write-up — not the source, and not a running system.

### What these repositories can actually tell you

How a problem was scoped. What was cut, and why. Whether the trade-off can be articulated afterwards. That is what each README documents, and it's the part that doesn't expire.

If you want to see how I write code today, look at what carries a current date. Older repositories show where I was, not where I am — which is true of everyone's.

I'm glad to bring any of this current if it's genuinely useful to you. Ask, and I will.

---

## 🚀 Most recent role

**Full-Stack AI Engineer — Esimtime** *(Jul 2025 – Aug 2026 · remote, US)* — **now concluded; open to new work**

Sole architect of a conversational commerce platform running the full eSIM lifecycle on WhatsApp and Telegram.

* Stateful **LangGraph** agent over **27 schema-validated tools**, >99% tool execution accuracy
* Hybrid **Qdrant** retrieval — server-side dense + sparse fusion with cross-encoder reranking, 15–25% relevance lift over single-method search
* Self-hosted speech (**faster-whisper**, **Piper**) — no per-minute billing, models chosen by measured latency/memory benchmarks
* Ten-layer security architecture built after a live exploitation attempt; held **300+ RPS** adversarial load with 100% legitimate-traffic success
* Ranked **Top 5 AI company on F6S** (May 2026) and Top 5 of 39 at an investor showcase

👉 **[Read the architecture case study](https://github.com/JoshPola96/enterprise-ai-agent-architecture-esim)**

---

## 🔨 Currently building

**[ai-data-agent](https://github.com/JoshPola96/ai-data-agent)** — a ReAct agent over your own documents, with no agent framework underneath. Six purpose-built tools, parallel execution, hybrid BM25+FAISS retrieval with cross-encoder reranking, and 429 offline tests. Ask a question about a spreadsheet in one language, get an answer and a chart back in another. Active work.

**Multi-agent narrative simulation (CrewAI)** — next up. A crew of adversarial agents improvising a story against each other, to see how far coherent long-form narrative survives when no single agent holds the plot. Mostly an excuse to push multi-agent coordination somewhere it isn't usually pointed.

---

## 📌 Selected work

| Project | What it demonstrates | Stack |
|---|---|---|
| **[ai-data-agent](https://github.com/JoshPola96/ai-data-agent)** | ReAct agent with no framework underneath — six tools, parallel execution, hybrid BM25+FAISS retrieval, 429 offline tests | FastAPI · FAISS · Redis · OpenAI/Gemini |
| **[company-bankruptcy-prediction-mlops](https://github.com/JoshPola96/company-bankruptcy-prediction-mlops)** | Drift-triggered automatic retraining — Evidently detects degradation, Airflow retrains, MLflow gates promotion | Airflow · MLflow · Terraform · AWS |
| **[rppg-monitor](https://github.com/JoshPola96/rppg-monitor)** | Heart rate, HRV and respiration from webcam video alone, streamed over WebSocket | MediaPipe · OpenCV · FastAPI |
| **[heart-attack-data-pipeline](https://github.com/JoshPola96/heart-attack-data-pipeline)** | Full ELT warehouse — infrastructure-as-code through to dashboard, nothing manual | GCP · dbt · BigQuery · Airflow |
| **[dissertation-racism-detection-bert-cnn-bilstm](https://github.com/JoshPola96/dissertation-racism-detection-bert-cnn-bilstm)** | The complete experimental record, including the branches that failed — multimodal BERT+CNN+BiLSTM with bias minimisation | TensorFlow · BERT |
| **[gloved-ungloved-yolov8](https://github.com/JoshPola96/gloved-ungloved-yolov8)** | Data-centric CV — CLIP and pose estimation cross-validate labels before a single epoch runs | YOLOv8 · CLIP · Streamlit |

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

## 🛠️ Background

Nine years across database engineering (SQL Server, ETL for US real estate), enterprise .NET (loan assessment migration at Permanent TSB, Dublin), early-stage backend (NestJS, Netherlands), and computer vision (YOLOv7 for ADAS at RoshAI).

Between the Dublin role and the return to tech I worked airside logistics at Dublin Airport (Garda-vetted, blue badge) and HACCP-regulated manufacturing in Ireland, self-funding relocation and retraining across 12-hour rotating night shifts. That's on the CV deliberately — it's where the execution discipline came from.

Also holds PG diplomas in Airport Cargo Management and Logistics & Supply Chain Management, which is how the eSIM-commerce domain stopped being unfamiliar territory.

**Languages** English (native) · Malayalam (native) · Hindi, Tamil, German (beginner)

---

⭐ Open to full-time, contract and freelance work. Happy to talk architecture, tradeoffs, or anything in the repos above — [get in touch](mailto:josh19peter96@gmail.com).

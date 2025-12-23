# 🚀 ZION — Future of Work Hackathon Entry

**One-liner:** An AI agent network that verifies developer skills from GitHub, detects hiring bias, and explains why candidates match jobs — all transparently, auditable, and developer-friendly. ⚡️

---

## 🔥 TL;DR
ZION replaces the hiring black box with a court of evidence. Developers prove skill with GitHub as the source of truth, AI explains *why* candidates match, and a bias detector calls out unfair filters — loud, proud, and transparent. 🍿

---

## 🧠 The Problem (In Plain Words)
- Great devs get rejected because screening is a black box. ⚫️
- Resumes compress truth; GitHub contains *work*. 🧾 → 🧠
- Bias in hiring is invisible and unmeasurable. ⚖️
- Candidates never know *why* they were rejected. 💬

ZION fixes that.

---

## 🎯 System Flow (Super Short)
1. Dev enters `github_username` → Skill Verifier analyzes public repos.
2. Verifier builds a **Skill Profile** (commits, PRs, tests, architecture signals).
3. Bias Detector evaluates pipeline + job filters → fairness score & fixes.
4. Match Explainer gives human-grade explanations + proof links.
5. Employer sees verified, explained candidate cards with audit trail.

---

## 🧰 Tech Stack
- **Frontend:** React + Tailwind CSS
- **Backend:** Node.js / Python FastAPI (microservices)
- **LLMs:** Claude API + OpenAI API for skill analysis & transparent explanations
- **Data:** GitHub API (repo analysis), static analysis tools, dependency graphs
- **DB:** MongoDB or Firebase
- **Optional:** IPFS / blockchain for immutable audit ledger

---

## ✨ Killer Features
- **Skill Verifier:** Maps repo signals to skill buckets (Frontend, Backend, DevOps, ML).
- **Bias Detector:** Quantifies bias per job posting and pipeline stage; suggests mitigations.
- **Match Explainer:** LLM-generated rationale with direct links to commits, PRs, and lines of code.
- **Transparency Ledger:** Immutable audit logs of decisions and scores.
- **Candidate Portal:** Candidates view exactly which artifacts affected their score.
- **Employer Dashboard:** Filter by verified skills, fairness score, and explainability index.

---

## 🧪 Example Outputs
**Skill profile (short):**

```json
{
  "username": "alice-dev",
  "skills": {"python": 0.92, "react": 0.78, "testing": 0.85},
  "evidence": [
    {"repo":"microservice-xyz","file":"auth.py","commit":"abc123","reason":"solid auth design, tests"},
    {"repo":"ui-kit","file":"Button.jsx","commit":"def456","reason":"accessible, reusable"}
  ],
  "skill_score": 0.85
}
```

**Bias report (short):**

```json
{
  "job_id":"backend-senior-01",
  "bias_score":0.12,
  "flags":["gendered_language_in_desc","school_filter_overweight"],
  "recommendations":["remove_school_filter","display_skill_challenges"]
}
```

**Match explanation (short):**

> Candidate matches because their recent microservice PRs implemented idempotent APIs with tests, they have extensive integration tests, and multiple approved reviews from senior contributors.

---

## 🚀 Quickstart (Hackathon Mode)
**Prereqs:** Node, Python, pip, MongoDB or Firebase, Git

1. Clone
```bash
git clone https://github.com/TeamZION/zion-hackathon.git
cd zion-hackathon
```

2. Create `.env` with keys (example):
```
GITHUB_TOKEN=ghp_xxx
CLAUDE_API_KEY=claude_xxx
OPENAI_API_KEY=sk-xxx
MONGO_URI=mongodb://...
```

3. Run backend (FastAPI example):
```bash
cd backend
pip install -r requirements.txt
uvicorn app.main:app --reload --port 8000
```

4. Run frontend:
```bash
cd frontend
npm install
npm start
```

5. Try endpoints:
```
GET /api/verify/{github_username}
GET /api/bias/{job_id}
POST /api/explain { candidate: "username", job_id: "..." }
```

---

## 🧪 Demo Script (2 minutes)
1. Enter `alice-dev` in the search box → watch the Verifier parse repos and show "Skill Stamps". 🔧
2. Click "Explain match" → see an LLM-crafted reason with direct evidence links. 🔗
3. Run bias check for a job → get flags and suggested quick fixes. 🚨

---

## 🛡️ Privacy, Ethics & Governance
- Minimal profile data retained; candidate consent required before employers view results. ✅
- Bias metric is multi-faceted (statistical + simulation) — not just single proxies. ⚖️
- Roadmap: DAO-style governance for fairness rules and community-sourced fairness recipes. 🗳️

---

## 🌙 Roadmap & Moonshots
- **Phase 1 (MVP):** Skill Verifier, Match Explainer, Bias Detector — core hackathon build. ✅
- **Phase 2:** DAO governance, provable skill badges on-chain. ⛓️
- **Phase 3:** Integrations with ATS, real-time interview sandbox, multi-modal artifacts. 🛰️

---

## 🤝 Contributing
- PRs welcome. See `CONTRIBUTING.md`. Use feature branches: `feat/verifier-awesome` → PR → tag `hackathon/entry`.

---

## 🧨 Hype Section (Because You Asked for CRAZY)
> This README is not shy. ZION will roast bad hiring rules, give receipts for every opinion, and make hiring teams sweat (in a good way). Bring popcorn. 🍿

---

## 🧾 License
MIT © Team ZION

---

## 📬 Contact
Demo link: https://zion-hackathon.demo (placeholder)
Email: team@zion.example — subject: "I want ZION in my hiring stack"

---

If you'd like, I can also add automated demo data, a one-click deploy script (Docker + Fly/Heroku), or generate LLM prompt templates for `ExplainMatch`, `BiasAudit`, and `SkillExtract`. Say the word and I’ll add it. ✨

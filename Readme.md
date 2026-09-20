# Pulsar: AI-Powered Open-Source Issue Triaging & Dependency Health Sentinel

Pulsar is an automated, low-latency intelligence layer designed for open-source maintainers. It connects to GitHub repositories, automatically parses and categorizes incoming issues, flags duplicate bug reports via semantic matching, and computes a dynamic Dependency Health Score.

---

## Key Features
- **Issue Ingestion & Auto-Triage:** Automatically tags issues (`Bug`, `Feature`, `Documentation`, `Security`), determines severity (`Low`, `Medium`, `High`, `Critical`), and suggests immediate maintainer actions.
- **Semantic Duplicate Detection:** Compares incoming issues with historical repository tickets using semantic embeddings and similarity metrics.
- **Dependency Health Sentinel:** Scans `package.json` / `requirements.txt` to calculate an overall Repository Health Score (0–100%) and highlights outdated or vulnerable packages.
- **Maintainer Action Panel:** 1-click copyable markdown responses ready to post on GitHub.

---

## Tech Stack
- **Framework:** Next.js (App Router) & React
- **Language:** TypeScript
- **Styling:** Tailwind CSS & Lucide React
- **Visuals:** Recharts
- **Integrations:** Google Gemini API & GitHub REST API (@octokit/rest)

---

## Getting Started

### 1. Configure Environment Variables
Create a `.env.local` file in the root directory:
```env
GITHUB_TOKEN=your_github_token_here
GEMINI_API_KEY=your_gemini_api_key_here
```

### 2. Install Dependencies & Run
```bash
npm install
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) to view Pulsar.

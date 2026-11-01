# Everton Resende

**AI Engineer.** I build LLM, agent and RAG systems and ship them to production, from architecture to infrastructure, with TypeScript, Python, Cloudflare and AWS. 7+ years in software development.

Open to remote work: international contracts, B2B contractor work, or full-time employment in Brazil (CLT).

[evertonresende.com](https://evertonresende.com/en) · [CV (PDF)](https://evertonresende.com/cv-everton-resende-en.pdf) · [LinkedIn](https://www.linkedin.com/in/evertonresende) · [everton.augustor@gmail.com](mailto:everton.augustor@gmail.com)

## Public code

- [agent-evals-demo](https://github.com/evertonresende/agent-evals-demo): how I test an LLM support agent before a change ships. A golden set, metrics, an LLM judge checked against 26 hand labels, and a CI gate that fails on unsafe replies. Synthetic data.
- [portfolio-everton](https://github.com/evertonresende/portfolio-everton): source code for evertonresende.com. React 19 Server Components on Cloudflare Workers, built with coding agents.
- Cal.com: [#27636](https://github.com/calcom/cal.com/pull/27636) and [#27637](https://github.com/calcom/cal.com/pull/27637), both merged.

## What I've put into production

- **Tazz**, a ride-hailing app: a support agent with evals, guardrails and an LLM judge, where a person reviews every draft. Keeping the same model, a new prompt and guardrail raised passing eval cases from 10 to 23 of 31. [Case study](https://evertonresende.com/en/projects/tazz)
- **Dental Smart**, a SaaS used by ~20 dental clinics: Whisper transcribes the visit and Llama 3.3 70B writes the clinical note into the patient record, as a draft for the dentist to review. [Case study](https://evertonresende.com/en/projects/dental-smart)
- **Maximus**, an app for anesthesiologists: a clinical RAG chat on the OpenAI Responses API with file_search.
- **Coppay**, a fintech: LLM credit assessments with gpt-oss-120b at ~R$0.01 each. The analyst makes the call.
- **Rota Protegida**, face recognition for a city's schools: AuraFace embeddings in Cloudflare Vectorize, with AWS Rekognition for uncertain matches and human review after that.

Most of this code belongs to clients and is private. The Tazz and Dental Smart case studies cover the architecture and the decisions; the site covers the rest.

## How I work

I design the architecture and the acceptance criteria, coding agents write most of the code, and I review it, debug it and own what goes to production.

## Stack

- **AI:** OpenAI, Anthropic, Groq and Workers AI models · agents and tool calling · RAG · structured output · guardrails · LLM-as-judge · evals · speech-to-text
- **Code:** TypeScript, Python, SQL · Hono, FastAPI, Node.js · React, Next.js, React Native / Expo
- **Infra:** Cloudflare (Workers, Durable Objects, Queues, D1, R2, Vectorize, AI Gateway) · Postgres, Supabase · AWS · Docker · GitHub Actions

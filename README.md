# Giorgio Loguercio

**Software Engineer — LLM apps, RAG & evals.** TypeScript/Node · Python · Postgres.
Necochea, Argentina (UTC-3) · Open to remote work.

[Portfolio](https://giorgio-loguercio.vercel.app) · [LinkedIn](https://www.linkedin.com/in/corcho-log/) · [Email](mailto:loguerciogiorgioivan@gmail.com)

## What I build

**[Rekindle](https://github.com/Corcholog/rekindle)** — local-first assistant that links what you read to what you write.
Two-stage retrieval (pgvector pre-filter, then an LLM triage that answers with schema-validated JSON), a provider fallback
chain (DeepSeek, Gemini, local Ollama), stale-suggestion detection by vector drift, and an eval harness over a
hand-labeled dataset: Precision@K, Recall@K, triage F1, quality gates, per-token cost and latency telemetry, 426 tests
with Testcontainers. *TypeScript · Fastify · Postgres/pgvector · Drizzle · Ollama · DeepSeek/Gemini*

**[LIDE 2](https://github.com/Corcholog/lide2)** — the official platform of the RedUNCI inter-university League of Legends
tournament (113 players, 20 teams, 13 universities): standings, fixtures, playoffs, player and team profiles, and a match
replay parser with pro-style statistics. *Next.js · React · TypeScript · Supabase (Postgres, Auth, Storage, RLS) · Vercel*

**[My Merry May](https://github.com/Corcholog/mmm-spanish-patch)** — Spanish fan translation of a PS2 visual novel:
reverse-engineered the script format and the executable, built a screen simulator and byte-identical round-trip tests, and
ran the translation through a five-agent pipeline (scout, translator, automatic checks, reviewer, human review) with shared
memory across batches. *Python · reverse engineering · agents*

**[This portfolio](https://github.com/Corcholog/portfolio)** — bilingual (es/en), fully static. Typed content dictionaries
for both languages with a build-time parity gate that fails the build if the two drift apart. *Next.js 16 · React 19 · TypeScript · Tailwind v4*

## Looking for

A junior **AI Engineer** or **Software Engineer** role — remote or in Argentina — where I ship LLM features backed by
evaluations alongside production full-stack work.

## Background

Systems Engineering at UNICEN (2021–2026). Thesis on automatic fall detection from video: a comparative study of human
pose estimators and CNN-LSTM / TCN-Transformer / Transformer architectures with automated experimentation and
benchmarking pipelines. Also an ITBA Advanced Full-Stack certification (2025, on scholarship) and a Diploma in Esports at
UNLP (2026).

## How this is built

Most of the code above was written with AI agents as a pair programmer. The design decisions, the threat model, the
evaluation methodology and every number reported here are mine, and each repository keeps a build log (`docs/JOURNEY.md`)
with the decisions, the dead ends and the bugs found along the way.
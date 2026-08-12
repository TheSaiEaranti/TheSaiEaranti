<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,50:161b22,100:0d1117&height=120&section=header" width="100%" />

# Hi, I'm Sai <img src="https://media.giphy.com/media/hvRJCLFzcasrR4ia7z/giphy.gif" width="35">

[![UT Austin](https://img.shields.io/badge/Information_%26_Data_Science_%2B_AI_Minor_@_UT_Austin-BF5700?style=for-the-badge&logoColor=white)](https://www.utexas.edu/)

<p align="center">
  <a href="mailto:saipreetam.earanti@utexas.edu"><img src="https://img.icons8.com/color/48/gmail-new.png" width="32" alt="Email"/></a>
  <a href="https://www.linkedin.com/in/sai-preetam-earanti-580717285/"><img src="https://img.icons8.com/color/48/linkedin.png" width="32" alt="LinkedIn"/></a>
  <a href="https://thesaiearanti.github.io/"><img src="https://cdn.simpleicons.org/googlechrome/e6edf3" width="32" alt="Website"/></a>
  <a href="https://github.com/TheSaiEaranti"><img src="https://cdn.simpleicons.org/github/e6edf3" width="32" alt="GitHub"/></a>
</p>
</div>
<br>

## 🛠️ Open Source

Bugs and gaps I found by reading source in production AI infrastructure, fixed, and shipped upstream.

| Project | Contribution | Status |
| :--- | :--- | :--- |
| **[openai/openai-agents-python](https://github.com/openai/openai-agents-python/pull/3951)** <br> <sub>OpenAI Agents SDK · 28k+ ★</sub> | Sandbox `ls` parsing silently dropped every device node via a swallowed `ValueError`; fixed for both GNU and BSD formats. | ![Merged](https://img.shields.io/badge/merged-8957e5?style=flat-square) |
| **[facebookresearch/hydra](https://github.com/facebookresearch/hydra/pull/3315)** <br> <sub>Hydra config framework · 10k+ ★</sub> | Defaults-list overrides were first-write-wins where the docs promise last-wins; reworked with the lead maintainer to register overrides during the reverse tree traversal. | ![Merged](https://img.shields.io/badge/merged-8957e5?style=flat-square) |
| **[facebookresearch/hydra](https://github.com/facebookresearch/hydra/pull/3319)** <br> <sub>Hydra config framework · 10k+ ★</sub> | A dangling override was silently rescued by a command-line append, discarding the user's value; composition now fails identically with or without the append. | ![Merged](https://img.shields.io/badge/merged-8957e5?style=flat-square) |
| **[openai/openai-agents-python](https://github.com/openai/openai-agents-python/pull/3956)** <br> <sub>OpenAI Agents SDK · 28k+ ★</sub> | Tool schemas silently dropped `*args`/`**kwargs` descriptions for Google/NumPy docstrings — starred names never matched the bare-name lookup. | ![Merged](https://img.shields.io/badge/merged-8957e5?style=flat-square) |
| **[cloudflare/workers-sdk](https://github.com/cloudflare/workers-sdk/pull/14838)** <br> <sub>Wrangler CLI · 4k+ ★</sub> | `wrangler` hung unkillably during Access auth — a synchronous `spawnSync` froze the event loop so ctrl+c could never be processed. | ![Merged](https://img.shields.io/badge/merged-8957e5?style=flat-square) |
| **[cloudflare/workers-sdk](https://github.com/cloudflare/workers-sdk/pull/14847)** <br> <sub>Miniflare / Workflows · 4k+ ★</sub> | The local Workflows emulator double-executed duplicate deterministic IDs that production dedupes; `create` now throws and `createBatch` skips, per the documented contract. | ![Open](https://img.shields.io/badge/open-238636?style=flat-square) |
| **[awslabs/agent-plugins](https://github.com/awslabs/agent-plugins/pull/244)** <br> <sub>AWS agent plugins · 800+ ★</sub> | A duplicate JSON key silently discarded 45 AWS IoT shape names, making diagram validation reject legitimate shapes. | ![Open](https://img.shields.io/badge/open-238636?style=flat-square) |
| **[awslabs/agent-plugins](https://github.com/awslabs/agent-plugins/pull/245)** <br> <sub>AWS agent plugins · 800+ ★</sub> | 45 lint findings across 12 files down to zero, preserving the customer-facing template scaffolding autofix would have stripped. | ![Open](https://img.shields.io/badge/open-238636?style=flat-square) |
| **[redis/redis-vl-python](https://github.com/redis/redis-vl-python/pull/654)** <br> <sub>Redis Vector Library · 400+ ★</sub> | Documented the exception hierarchy from actual raise sites — the obvious example would have documented an exception that can never fire. | ![Merged](https://img.shields.io/badge/merged-8957e5?style=flat-square) |
| **[openai/openai-agents-python](https://github.com/openai/openai-agents-python/pull/3961)** <br> <sub>OpenAI Agents SDK · 28k+ ★</sub> | `@function_tool` crashed at decoration time on numpy-array defaults: sentinel compared with `==` instead of identity, per the `inspect` convention. | ![Merged](https://img.shields.io/badge/merged-8957e5?style=flat-square) |
| **[facebookresearch/hydra](https://github.com/facebookresearch/hydra/pull/3320)** <br> <sub>Hydra config framework · 10k+ ★</sub> | `ConfigStore.store(group="")` created an empty-string group that `--help` traversed forever, dying with `RecursionError`. | ![Merged](https://img.shields.io/badge/merged-8957e5?style=flat-square) |
| **[google-deepmind/optax](https://github.com/google-deepmind/optax/pull/1735)** <br> <sub>Optax (JAX optimizers) · 2k+ ★</sub> | `matrix_inverse_pth_root` silently returned matrices up to **18.6% wrong** for `p ∉ {1,2,4,8}` while reporting `1e-7` convergence; replaced with exact exponentiation-by-squaring. | ![Open](https://img.shields.io/badge/open-238636?style=flat-square) |
| **[angular/angular](https://github.com/angular/angular/pull/69955)** <br> <sub>Angular framework · 100k+ ★</sub> | `NgOptimizedImage` fired false-positive NG02952 bursts for cached images loading before DOM attachment; guarded the dev-mode check on `isConnected`. | ![Open](https://img.shields.io/badge/open-238636?style=flat-square) |
| **[google/flax](https://github.com/google/flax/pull/5537)** <br> <sub>Flax (JAX neural networks) · 7k+ ★</sub> | The new RoPE attention's `input_positions` crashed on every call — `vmap` mapped the sequence axis as a heads axis; broadcasting it also removed the branch. | ![Open](https://img.shields.io/badge/open-238636?style=flat-square) |
| **[google-deepmind/optax](https://github.com/google-deepmind/optax/pull/1736)** <br> <sub>Optax (JAX optimizers) · 2k+ ★</sub> | `optax.sm3` crashed with a bare `IndexError` on any scalar parameter; 0-d leaves now follow the algorithm's natural degenerate case. | ![Open](https://img.shields.io/badge/open-238636?style=flat-square) |
| **[cloudflare/workers-sdk](https://github.com/cloudflare/workers-sdk/pull/14865)** <br> <sub>Wrangler CLI · 4k+ ★</sub> | Local dev silently rewrites `request.url`/`Host`/`Origin` to the route host, breaking localhost CORS checks; exposed a documented `--infer-origin-from-routes` opt-out. | ![Open](https://img.shields.io/badge/open-238636?style=flat-square) |
| **[redis/redis-vl-python](https://github.com/redis/redis-vl-python/pull/655)** <br> <sub>Redis Vector Library · 400+ ★</sub> | `Timestamp != date(...)` returned exactly the day it was documented to exclude — the date branch built the same positive range as `==`. | ![Merged](https://img.shields.io/badge/merged-8957e5?style=flat-square) |
| **[cloudflare/cloudflare-docs](https://github.com/cloudflare/cloudflare-docs/pull/32497)** <br> <sub>Cloudflare docs · 4k+ ★</sub> | Documented the `--infer-origin-from-routes` flag for `wrangler dev`, requested by the reviewer of the companion workers-sdk PR. | ![Merged](https://img.shields.io/badge/merged-8957e5?style=flat-square) |

---

I like problems where the failure is invisible — silent data loss, a process that hangs instead of crashing, a model that's confidently wrong. Most of what I build sits at the intersection of LLM systems and infrastructure: agent orchestration, retrieval, and inference plumbing. Also interested in fintech, NLP, and sports analytics.

## Stack

<div align="center">

**`Languages`**
<br>
<img src="https://skillicons.dev/icons?i=python,ts,js,go,java" />

**`Frameworks`**
<br>
<img src="https://skillicons.dev/icons?i=fastapi,nextjs,react,nodejs,tailwind" />

**`Data & Tools`**
<br>
<img src="https://skillicons.dev/icons?i=postgres,sqlite,docker,git,github,vscode" />

<br>

<sub>Also: ChromaDB · sentence-transformers · Pydantic · Drizzle ORM · PixiJS · PGlite · Anthropic &amp; OpenAI SDKs</sub>

</div>

## Projects

| | |
| :--- | :--- |
| **[multi-agent-research-system](https://github.com/TheSaiEaranti/multi-agent-research-system)** | Orchestrator-worker multi-agent research system over ChromaDB. `Python` `FastAPI` |
| **[agent-canvas](https://github.com/TheSaiEaranti/agent-canvas)** | A visual canvas for composing and debugging AI agents. `TypeScript` `Next.js` |
| **[llm-inference-engine](https://github.com/TheSaiEaranti/llm-inference-engine)** | Agentic inference engine — streaming, tool use, multi-step agent loops, memory. `Python` `FastAPI` |
| **[living-city](https://github.com/TheSaiEaranti/living-city)** | Browser-based living city of NPCs with persistent memory. `TypeScript` `PixiJS` |
| **[grandmaster-ghost](https://github.com/TheSaiEaranti/grandmaster-ghost)** | A chess AI that attacks *and blunders* like a specific player, built from their real games. `Python` |
| **[sign-language-translator](https://github.com/TheSaiEaranti/sign-language-translator)** | Real-time ASL translator — MediaPipe hand tracking, hybrid letter + phrase models. `Python` |

<div align="center">

<table>
  <tr>
    <td>
      <img align="center" src="https://github-readme-stats.vercel.app/api?username=TheSaiEaranti&show_icons=true&theme=tokyonight&hide_title=true&include_all_commits=true&hide_border=true" />
    </td>
    <td>
      <img align="center" src="https://github-readme-stats.vercel.app/api/top-langs/?username=TheSaiEaranti&layout=compact&theme=tokyonight&hide_title=true&hide_border=true&exclude_repo=helphub,TheSaiEaranti" />
    </td>
  </tr>
</table>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,50:161b22,100:0d1117&height=100&section=footer" width="100%" />
</div>

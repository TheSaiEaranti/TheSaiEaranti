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
| **[openai/openai-agents-python](https://github.com/openai/openai-agents-python/pull/3951)** <br> <sub>OpenAI Agents SDK · 28k+ ★</sub> | Sandbox directory listings silently dropped every device node — a swallowed `ValueError` discarded entries with no error at all. Fixed across **both** GNU and BSD `ls` formats after review surfaced a macOS-only gap. | ![Merged](https://img.shields.io/badge/merged-8957e5?style=flat-square) |
| **[facebookresearch/hydra](https://github.com/facebookresearch/hydra/pull/3315)** <br> <sub>Hydra config framework · 10k+ ★</sub> | A defaults-list override in an appended config was silently ignored whenever the primary config already overrode that group — first-write-wins where the docs promise last-wins. Reworked after review from the lead maintainer: registration moved into the reverse tree traversal so first-registered = last-in-depth-first-order, plus an append edge case his prescribed approach missed — caught by stress-testing 67 compositions before pushing. Merged same-day after the rework; the maintainer filed the follow-up issue it surfaced and invited milestone contributions. | ![Merged](https://img.shields.io/badge/merged-8957e5?style=flat-square) |
| **[facebookresearch/hydra](https://github.com/facebookresearch/hydra/pull/3319)** <br> <sub>Hydra config framework · 10k+ ★</sub> | Follow-up the maintainer filed off my previous PR's review: a dangling defaults-list override (no target group) was silently rescued by a command-line append, discarding the user's appended value. Made composition fail-fast identically with or without the append. | ![Open](https://img.shields.io/badge/open-238636?style=flat-square) |
| **[openai/openai-agents-python](https://github.com/openai/openai-agents-python/pull/3956)** <br> <sub>OpenAI Agents SDK · 28k+ ★</sub> | Google and NumPy docstrings write variadics with stars (`*args:`, `**kwargs:`); griffe returns those names verbatim, but schema lookup used bare names — so tool schemas silently dropped those parameter descriptions in two of three supported styles. Found by cross-checking the three styles against each other; merged within hours. | ![Merged](https://img.shields.io/badge/merged-8957e5?style=flat-square) |
| **[cloudflare/workers-sdk](https://github.com/cloudflare/workers-sdk/pull/14838)** <br> <sub>Wrangler CLI · 4k+ ★</sub> | `wrangler` hung unkillably during Cloudflare Access auth: a synchronous `spawnSync` froze Node's event loop, so raw-mode ctrl+c keypresses could never be processed. Converted to an async spawn with exit-hook cleanup. | ![Open](https://img.shields.io/badge/open-238636?style=flat-square) |
| **[cloudflare/workers-sdk](https://github.com/cloudflare/workers-sdk/pull/14847)** <br> <sub>Miniflare / Workflows · 4k+ ★</sub> | The local Workflows emulator ignored the documented deterministic-ID idempotency contract — duplicate creates double-executed workflow bodies, so the exact code pattern the docs recommend for queue-driven idempotency passed local tests while validating the wrong behavior. Made `create` throw and `createBatch` dedupe, with existence decided inside the engine Durable Object for cross-isolate consistency. | ![Open](https://img.shields.io/badge/open-238636?style=flat-square) |
| **[awslabs/agent-plugins](https://github.com/awslabs/agent-plugins/pull/244)** <br> <sub>AWS agent plugins · 800+ ★</sub> | A duplicate `iot` key in the draw.io shape registry meant every JSON parser kept the second block and silently discarded 45 shape names — so diagram validation rejected legitimate AWS IoT shapes. Filed as a lint failure; it was breaking real validation. | ![Open](https://img.shields.io/badge/open-238636?style=flat-square) |
| **[awslabs/agent-plugins](https://github.com/awslabs/agent-plugins/pull/245)** <br> <sub>AWS agent plugins · 800+ ★</sub> | 45 lint findings across 12 files, down to zero. The issue's file list had gone stale — one error class had moved entirely into a sibling issue's scope. Kept the customer-facing templates' deliberate scaffolding instead of letting autofix strip it. | ![Open](https://img.shields.io/badge/open-238636?style=flat-square) |
| **[redis/redis-vl-python](https://github.com/redis/redis-vl-python/pull/654)** <br> <sub>Redis Vector Library · 400+ ★</sub> | Documented the exception hierarchy by tracing every class to its actual raise site rather than the class list. `SchemaValidationError` only fires with `validate_on_load=True`, so the obvious example would have documented an exception that can never be raised. | ![Open](https://img.shields.io/badge/open-238636?style=flat-square) |

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

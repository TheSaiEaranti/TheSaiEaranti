<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,50:161b22,100:0d1117&height=120&section=header" width="100%" />

# Hi, I'm Sai <img src="https://media.giphy.com/media/hvRJCLFzcasrR4ia7z/giphy.gif" width="35">

[![UT Austin](https://img.shields.io/badge/Information & Data Science_%2B_AI_Minor_@_UT_Austin-BF5700?style=for-the-badge&logoColor=white)](https://www.utexas.edu/)

<p align="center">
  <a href="mailto:saipreetam.earanti@utexas.edu"><img src="https://img.icons8.com/color/48/gmail-new.png" width="32" alt="Email"/></a>
  <a href="https://www.linkedin.com/in/sai-preetam-earanti-580717285/"><img src="https://img.icons8.com/color/48/linkedin.png" width="32" alt="LinkedIn"/></a>
  <a href="https://thesaiearanti.github.io/"><img src="https://cdn.simpleicons.org/googlechrome/e6edf3" width="32" alt="Website"/></a>
  <a href="https://github.com/TheSaiEaranti"><img src="https://cdn.simpleicons.org/github/e6edf3" width="32" alt="GitHub"/></a>
</p>
</div>
<br>

## 🛠️ Open Source

Bugs I found by reading source in production AI infrastructure, fixed, and shipped upstream.

| Project | Contribution | Status |
| :--- | :--- | :--- |
| **[openai/openai-agents-python](https://github.com/openai/openai-agents-python/pull/3951)** <br> <sub>OpenAI Agents SDK · 28k+ ★</sub> | Sandbox directory listings silently dropped every device node — a swallowed `ValueError` discarded entries with no error at all. Fixed across **both** GNU and BSD `ls` formats after review surfaced a macOS-only gap. | ![Merged](https://img.shields.io/badge/merged-8957e5?style=flat-square) |
| **[cloudflare/workers-sdk](https://github.com/cloudflare/workers-sdk/pull/14838)** <br> <sub>Wrangler CLI · 4k+ ★</sub> | `wrangler` hung unkillably during Cloudflare Access auth: a synchronous `spawnSync` froze Node's event loop, so raw-mode ctrl+c keypresses could never be processed. Converted to an async spawn with exit-hook cleanup. | ![Open](https://img.shields.io/badge/open-238636?style=flat-square) |

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

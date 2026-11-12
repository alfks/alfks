<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:193E45,100:3E8E7E&height=190&section=header&text=alfks&fontSize=64&fontColor=F5F4EE&fontAlignY=36&desc=Building%20AI%20agents%20that%20work%20with%20people&descSize=18&descAlignY=58" width="100%" alt="alfks" />

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=18&duration=2600&pause=900&color=3E8E7E&center=true&vCenter=true&width=520&lines=AI+Agent+Engineer+%40+Telicity;LangGraph+%E2%80%A2+RAG+%E2%80%A2+Knowledge+Graph;NAVER+Boostcamp+AI+Tech+8th+%E2%80%94+NLP" alt="typing" />

<p><a href="https://telicity.ai"><img src="https://img.shields.io/badge/Telicity-193E45?style=for-the-badge&logo=googlechrome&logoColor=white" /></a>&nbsp;<a href="https://github.com/boostcampaitech8"><img src="https://img.shields.io/badge/Boostcamp_AI_Tech_8-03C75A?style=for-the-badge&logo=naver&logoColor=white" /></a></p>

<br/>

### 👋 사람과 **함께** 일하는 AI 에이전트를 만듭니다

I build AI agents that work *with* people.

🧠 **Telicity** — AI twin agent system &nbsp;·&nbsp; 🔗 Agents · RAG · Knowledge Graph · LLM pipelines

</div>

<br/>

## 🚀 Projects

| Project | Period | Role | Remarks |
| :-- | :-- | :-- | :-- |
| 🧠 **[Telicity](https://telicity.ai)** | `2026.06~now` | **Co-founder · AI Engineer** | AI twin agent system · #1 contributor (3.6K+ commits) |
| 🏆 **[Mit](https://github.com/boostcampaitech8/pro-nlp-finalproject-nlp-14)** | `2026.01~2026.03` | **Agent orchestration lead** | LangGraph agent · Text2Cypher on Neo4j · SSE streaming · LLM-as-judge |
| 📝 **[Korean CSAT QA](https://github.com/boostcampaitech8/pro-nlp-generationfornlp-nlp-14)** | `2025.12~2026.01` | **Data & RAG** | Leak-free GroupKFold · option shuffling · Korean-history RAG + reranker |
| 📚 **[MRC / ODQA](https://github.com/boostcampaitech8/pro-nlp-mrc-nlp-14)** | `2025.12` | **Retrieval** | 🎯 Public EM **75.83** · MeCab BM25 + BGE-M3 hybrid · coverage 77% → 99.97% |
| 📰 **[News Fit](https://github.com/alfks/news-fit-mvp)** | `2025.11~2026.07` | **RAG & LoRA fine-tuning** | News tone re-framing · RAG fact anchoring · LoRA (PEFT + TRL) |
| 🔎 **[Semantic Search](https://github.com/alfks/SemanticSearch_Project)** | `2024.03~2025.02` | **Hybrid search & reranking** | E-commerce product search · BM25 + BGE-M3 (FAISS) · cross-encoder reranker |

<details>
<summary><b>🧠 Telicity — details</b></summary>
<br/>

| Area | What I did |
| :-- | :-- |
| 🧠 **Memory** | Per-user long-term memory: extracts event sentences from chats, groups them nightly, and serves a memory graph |
| 🙋 **Human-in-the-loop** | `ask_user` questions in chat, approval rules and human-decision routes before the agent acts |
| 🖥️ **PC agent** | Local executor with a workspace registry, forbidden paths and file / PDF / report tools |
| 📚 **Knowledge** | Grounded wiki answers with contradiction checks, and a knowledge-graph explorer screen |
| 🔐 **Privacy & security** | PII redaction and pseudonymization, agent sandbox (macOS Seatbelt, egress allowlist), prompt-injection rules |
| 📊 **Evals** | Memory-retrieval benchmark (own 60-question set + LoCoMo), router and tool-mapping eval sets |

<sub>3.6K+ commits · 975 feat · 932 fix · 301 test</sub>

</details>

<details>
<summary><b>🏆 Mit — details</b></summary>
<br/>

| Area | What I did |
| :-- | :-- |
| 🧩 **Orchestration** | Built the LangGraph agent (planner · executor · tools · response), then split it into voice and chat graphs |
| 🔎 **Search** | Moved meeting search to LLM-generated Cypher on Neo4j, kept it in sync with the schema |
| ⚡ **Real-time** | Token streaming over SSE, chat and TTS routed separately |
| 🚦 **Speed & cost** | Short-path router for simple questions (CLOVA Studio Router), task-specific HyperCLOVA X models |
| ✍️ **Prompts** | Role · constraint prompts, few-shot examples, guide mode |
| 📈 **Quality** | Langfuse tracing, GPT-4o LLM-as-a-judge rubric |

<sub>138 commits · 25 PRs</sub>

</details>

<details>
<summary><b>📝 Korean CSAT QA — details</b></summary>
<br/>

| Area | What I did |
| :-- | :-- |
| 🧪 **Validation** | StratifiedGroupKFold by passage group, so questions sharing a passage never leak across splits |
| 🔀 **Bias fix** | Found answers skewed to option 1 and applied option shuffling to remove position bias |
| 🔍 **Data forensics** | Traced data back to its sources (KLUE-MRC, MMMLU) and showed short passages (≤ 600 chars) need outside knowledge → RAG routing |
| 📚 **RAG DB** | Korean-history corpus end to end: crawling, Hanja-aware preprocessing, chunking, indexing |
| 🎯 **Reranker** | Added a reranker to the retrieval step at inference |

<sub>30 commits · 6 PRs</sub>

</details>

<details>
<summary><b>📚 MRC / ODQA — details</b></summary>
<br/>

| Area | What I did |
| :-- | :-- |
| 🔍 **EDA** | Found answers clustered at the start of passages and a topic imbalance (history / politics) |
| 🧪 **Leakage** | Spotted passages shared between train and validation, re-split by context ID |
| ✂️ **Chunking** | Sliding window (500 / overlap 128) raised document coverage from 77% to 99.97% |
| 🔀 **Hybrid retrieval** | MeCab-tokenized BM25 + BGE-M3 dense retrieval with FAISS |
| 🎯 **Result** | Public leaderboard EM 75.83 |

<sub>10 commits · 5 PRs</sub>

</details>

<details>
<summary><b>📰 News Fit — details</b></summary>
<br/>

| Area | What I did |
| :-- | :-- |
| 🔍 **RAG** | Built the retrieval step on ChromaDB: anchors the article's facts and pulls in the other side's key argument |
| ✍️ **LoRA fine-tuning** | Trained per-stance LoRA adapters with PEFT + TRL to rewrite the tone |
| 🔁 **Pipeline** | Frame diagnosis → retrieval → generation → validation, regenerating when a result fails |

<sub>Streamlit demo</sub>

</details>

<details>
<summary><b>🔎 Semantic Search — details</b></summary>
<br/>

| Area | What I did |
| :-- | :-- |
| 🔀 **Hybrid search** | Combined TF-IDF / BM25 with BGE-M3 + FAISS, so both vague queries and exact product names are found |
| 🎯 **Reranking** | Added a cross-encoder reranker to reorder results by intent, beyond plain cosine similarity |
| 🛒 **Data** | Product data crawled from an e-commerce site (500 products × 21 fields) |

<sub>Team of 3</sub>

</details>


<br/>

## 📄 Publication

| Paper | Venue | Date | Role | Remarks |
| :-- | :-- | :-- | :-- | :-- |
| 📄 **[피처 맞춤 모델링을 통한 인기 유튜브 채널 특성 유형화 프레임워크](https://www.dbpia.co.kr/journal/articleDetail?nodeId=NODE11714648)**<br/><sub>최보현, 김고은, **문미란**, 박나예, 정은지, 채규현, 최예림</sub> | HCI Korea 2024<br/><sub>pp. 224–230</sub> | `2024.01` | **Co-author** (team of 7) | Capstone `2023.09~2024.02` · 997 YouTube channels clustered by topic · thumbnail · upload timing · LDA · Faster R-CNN · K-Means |

<details>
<summary><b>📺 YouTube Trend Framework (capstone) — details</b></summary>
<br/>

| Step | What we did |
| :-- | :-- |
| 📥 **Data** | 997 channels (500K+ subscribers) and 339K videos |
| 🧮 **Features** | Upload interval, video length, Shorts ratio |
| 🏷️ **Typing** | Topics with LDA, thumbnails with Faster R-CNN, upload time slots with KL divergence + K-Means |
| ✅ **Result** | Good clustering by silhouette score → published at HCI Korea 2024 |

<sub>Capstone · team of 7</sub>

</details>

<br/>

## 🏆 Awards

| Award | Contest | Date | Remarks |
| :-- | :-- | :-- | :-- |
| 🥇 **대상 (Grand Prize)** | KMR 빅데이터 센터 데이터 활용 아이디어 공모전 | `2023.12.13` | 중소기업 맞춤형 스마트팩토리 지표 · PCA + clustering (K-Means · GMM · hierarchical) |

<br/>

## 🎓 Education & 📜 Certifications

| When | | |
| :-- | :-- | :-- |
| `2021.03 – 2026.02` | 🏫 **Seoul Women's University** | B.S. Data Science |
| `2024.11` | 📊 **ADsP** | 데이터분석 준전문가 |
| `2025.04` | 🗄️ **SQLD** | SQL 개발자 |
| `2025.09 – 2026.03` | 🚀 **NAVER Boostcamp AI Tech 8th** | NLP track |

<br/>

## 🛠 Tech Stack

<div align="center">

<img src="https://skillicons.dev/icons?i=py,ts,js,pytorch,fastapi,nextjs,react&theme=dark" /><br/>
<img src="https://skillicons.dev/icons?i=postgres,cloudflare,vercel,docker,kubernetes,linux&theme=dark" /><br/>
<img src="https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square&logo=langchain&logoColor=white" /> <img src="https://img.shields.io/badge/Hugging_Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black" /> <img src="https://img.shields.io/badge/HyperCLOVA_X-03C75A?style=flat-square&logo=naver&logoColor=white" /> <img src="https://img.shields.io/badge/Claude_Code-D97757?style=flat-square&logo=anthropic&logoColor=white" />
<br/><br/>

**🕸️ Knowledge Graph**<br/>
<img src="https://img.shields.io/badge/Neo4j-4581C3?style=for-the-badge&logo=neo4j&logoColor=white" /> <img src="https://img.shields.io/badge/Cypher-008CC1?style=for-the-badge&logo=neo4j&logoColor=white" /> <img src="https://img.shields.io/badge/Text2Cypher-6A1B9A?style=for-the-badge" /> <img src="https://img.shields.io/badge/GraphRAG-3E8E7E?style=for-the-badge" /> <img src="https://img.shields.io/badge/Graph_Modeling-193E45?style=for-the-badge" />

</div>

<br/>

<div align="center">
  <img src="https://streak-stats.demolab.com?user=alfks&theme=transparent&hide_border=true&ring=3E8E7E&fire=3E8E7E&currStreakLabel=3E8E7E&sideLabels=8B949E&dates=8B949E&stroke=30363D" />
</div>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:3E8E7E,100:193E45&height=100&section=footer" width="100%" />

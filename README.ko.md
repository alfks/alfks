<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:193E45,100:3E8E7E&height=190&section=header&text=alfks&fontSize=64&fontColor=F5F4EE&fontAlignY=36&desc=Building%20AI%20agents%20that%20work%20with%20people&descSize=18&descAlignY=58" width="100%" alt="alfks" />

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=18&duration=2600&pause=900&color=3E8E7E&center=true&vCenter=true&width=520&lines=AI+Agent+Engineer+%40+Telicity;LangGraph+%E2%80%A2+RAG+%E2%80%A2+Knowledge+Graph;NAVER+Boostcamp+AI+Tech+8th+%E2%80%94+NLP" alt="typing" />

<p><a href="https://telicity.ai"><img src="https://img.shields.io/badge/Telicity-193E45?style=for-the-badge&logo=googlechrome&logoColor=white" /></a>&nbsp;<a href="https://github.com/boostcampaitech8"><img src="https://img.shields.io/badge/Boostcamp_AI_Tech_8-03C75A?style=for-the-badge&logo=naver&logoColor=white" /></a></p>

<p><a href="https://github.com/alfks/alfks/blob/HEAD/README.md">English</a> &nbsp;|&nbsp; <b>한국어</b></p>

<br/>

### 👋 사람과 **함께** 일하는 AI 에이전트를 만듭니다

🧠 **Telicity** — AI 트윈 에이전트 시스템 &nbsp;·&nbsp; 🔗 에이전트 · RAG · 지식 그래프 · LLM 파이프라인

</div>

<br/>

## 🚀 프로젝트

| 프로젝트 | 기간 | 역할 | 비고 |
| :-- | :-- | :-- | :-- |
| 🧠 **[Telicity](https://telicity.ai)** | `2026.06~현재` | **공동창업자 · AI 엔지니어** | AI 트윈 에이전트 시스템 · 기여도 1위 (3.6K+ 커밋) |
| 🏆 **[Mit](https://github.com/boostcampaitech8/pro-nlp-finalproject-nlp-14)** | `2026.01~2026.03` | **에이전트 오케스트레이션 리드** | LangGraph 에이전트 · Neo4j 기반 Text2Cypher · SSE 스트리밍 · LLM-as-judge |
| 📝 **[수능형 QA](https://github.com/boostcampaitech8/pro-nlp-generationfornlp-nlp-14)** | `2025.12~2026.01` | **데이터 & RAG** | 누수 없는 GroupKFold · 선택지 셔플링 · 한국사 RAG + 리랭커 |
| 📚 **[MRC / ODQA](https://github.com/boostcampaitech8/pro-nlp-mrc-nlp-14)** | `2025.12` | **검색(Retrieval)** | 🎯 Public EM **75.83** · MeCab BM25 + BGE-M3 하이브리드 · 커버리지 77% → 99.97% |
| 📰 **[News Fit](https://github.com/alfks/news-fit-mvp)** | `2025.11~2026.07` | **RAG & LoRA 파인튜닝** | 뉴스 논조 리프레이밍 · RAG 기반 사실 고정 · LoRA (PEFT + TRL) |
| 🔎 **[Semantic Search](https://github.com/alfks/SemanticSearch_Project)** | `2024.03~2025.02` | **하이브리드 검색 & 리랭킹** | 이커머스 상품 검색 · BM25 + BGE-M3 (FAISS) · 크로스 인코더 리랭커 |

<details>
<summary><b>🧠 Telicity — 상세 내용</b></summary>
<br/>

| 영역 | 담당 업무 |
| :-- | :-- |
| 🧠 **메모리** | 사용자별 장기 기억: 대화에서 사건 문장을 추출해 매일 밤 묶고, 메모리 그래프로 제공 |
| 🙋 **Human-in-the-loop** | 채팅 내 `ask_user` 질문, 에이전트 실행 전 승인 규칙과 사람이 결정하는 경로 |
| 🖥️ **PC 에이전트** | 워크스페이스 레지스트리, 접근 금지 경로, 파일 / PDF / 리포트 도구를 갖춘 로컬 실행기 |
| 📚 **지식** | 모순 검사를 거친 근거 기반 위키 답변, 지식 그래프 탐색 화면 |
| 🔐 **개인정보 & 보안** | 개인정보(PII) 마스킹 및 가명 처리, 에이전트 샌드박스 (macOS Seatbelt, 외부 통신 허용 목록), 프롬프트 인젝션 대응 규칙 |
| 📊 **평가** | 메모리 검색 벤치마크 (자체 60문항 세트 + LoCoMo), 라우터·도구 매핑 평가 세트 |

<sub>3.6K+ 커밋 · feat 975 · fix 932 · test 301</sub>

</details>

<details>
<summary><b>🏆 Mit — 상세 내용</b></summary>
<br/>

| 영역 | 담당 업무 |
| :-- | :-- |
| 🧩 **오케스트레이션** | LangGraph 에이전트(planner · executor · tools · response)를 구축한 뒤, 음성 그래프와 채팅 그래프로 분리 |
| 🔎 **검색** | 회의 검색을 Neo4j 위에서 LLM이 생성한 Cypher로 수행하도록 전환하고, 스키마와 동기화 유지 |
| ⚡ **실시간** | SSE 기반 토큰 스트리밍, 채팅과 TTS를 별도 경로로 처리 |
| 🚦 **속도 & 비용** | 단순 질문용 단축 경로 라우터 (CLOVA Studio Router), 작업별 HyperCLOVA X 모델 사용 |
| ✍️ **프롬프트** | 역할 · 제약 조건 프롬프트, few-shot 예시, 가이드 모드 |
| 📈 **품질** | Langfuse 트레이싱, GPT-4o LLM-as-a-judge 평가 루브릭 |

<sub>138 커밋 · 25 PR</sub>

</details>

<details>
<summary><b>📝 수능형 QA — 상세 내용</b></summary>
<br/>

| 영역 | 담당 업무 |
| :-- | :-- |
| 🧪 **검증** | 지문 그룹 기준 StratifiedGroupKFold로, 같은 지문을 공유하는 문제가 분할 사이에 새지 않도록 설계 |
| 🔀 **편향 수정** | 정답이 1번 선택지에 쏠린 것을 발견하고, 선택지 셔플링으로 위치 편향 제거 |
| 🔍 **데이터 추적** | 데이터 출처(KLUE-MRC, MMMLU)를 역추적하고, 짧은 지문(600자 이하)은 외부 지식이 필요함을 밝혀 RAG 라우팅으로 연결 |
| 📚 **RAG DB** | 한국사 코퍼스 전 과정 구축: 크롤링, 한자를 고려한 전처리, 청킹, 인덱싱 |
| 🎯 **리랭커** | 추론 시 검색 단계에 리랭커 추가 |

<sub>30 커밋 · 6 PR</sub>

</details>

<details>
<summary><b>📚 MRC / ODQA — 상세 내용</b></summary>
<br/>

| 영역 | 담당 업무 |
| :-- | :-- |
| 🔍 **EDA** | 정답이 지문 앞부분에 몰려 있고 주제(역사 / 정치)가 불균형함을 발견 |
| 🧪 **데이터 누수** | 학습·검증 세트가 공유하는 지문을 찾아내 context ID 기준으로 재분할 |
| ✂️ **청킹** | 슬라이딩 윈도우(500 / overlap 128)로 문서 커버리지를 77%에서 99.97%로 향상 |
| 🔀 **하이브리드 검색** | MeCab 토크나이징 BM25 + FAISS 기반 BGE-M3 dense 검색 |
| 🎯 **결과** | Public 리더보드 EM 75.83 |

<sub>10 커밋 · 5 PR</sub>

</details>

<details>
<summary><b>📰 News Fit — 상세 내용</b></summary>
<br/>

| 영역 | 담당 업무 |
| :-- | :-- |
| 🔍 **RAG** | ChromaDB 기반 검색 단계 구축: 기사의 사실관계를 고정하고 반대 측의 핵심 논거를 함께 가져옴 |
| ✍️ **LoRA 파인튜닝** | PEFT + TRL로 입장별 LoRA 어댑터를 학습해 논조를 재작성 |
| 🔁 **파이프라인** | 프레임 진단 → 검색 → 생성 → 검증, 검증을 통과하지 못하면 재생성 |

<sub>Streamlit 데모</sub>

</details>

<details>
<summary><b>🔎 Semantic Search — 상세 내용</b></summary>
<br/>

| 영역 | 담당 업무 |
| :-- | :-- |
| 🔀 **하이브리드 검색** | TF-IDF / BM25와 BGE-M3 + FAISS를 결합해, 모호한 질의와 정확한 상품명을 모두 검색 |
| 🎯 **리랭킹** | 단순 코사인 유사도를 넘어 의도에 맞게 결과를 재정렬하는 크로스 인코더 리랭커 추가 |
| 🛒 **데이터** | 이커머스 사이트에서 크롤링한 상품 데이터 (상품 500개 × 필드 21개) |

<sub>3인 팀</sub>

</details>

<br/>

## 📄 논문

| 논문 | 학회 | 날짜 | 역할 | 비고 |
| :-- | :-- | :-- | :-- | :-- |
| 📄 **[피처 맞춤 모델링을 통한 인기 유튜브 채널 특성 유형화 프레임워크](https://www.dbpia.co.kr/journal/articleDetail?nodeId=NODE11714648)**<br/><sub>최보현, 김고은, **문미란**, 박나예, 정은지, 채규현, 최예림</sub> | HCI Korea 2024<br/><sub>pp. 224–230</sub> | `2024.01` | **공동 저자** (7인 팀) | 캡스톤 `2023.09~2024.02` · 유튜브 채널 997개를 주제 · 썸네일 · 업로드 시점으로 군집화 · LDA · Faster R-CNN · K-Means |

<details>
<summary><b>📺 유튜브 트렌드 프레임워크 (캡스톤) — 상세 내용</b></summary>
<br/>

| 단계 | 진행 내용 |
| :-- | :-- |
| 📥 **데이터** | 채널 997개 (구독자 50만 명 이상), 영상 33.9만 개 |
| 🧮 **피처** | 업로드 간격, 영상 길이, 쇼츠 비율 |
| 🏷️ **유형화** | LDA로 주제, Faster R-CNN으로 썸네일, KL divergence + K-Means로 업로드 시간대를 유형화 |
| ✅ **결과** | 실루엣 점수 기준 우수한 군집화 → HCI Korea 2024 게재 |

<sub>캡스톤 · 7인 팀</sub>

</details>

<br/>

## 🏆 수상

| 수상 | 대회 | 날짜 | 비고 |
| :-- | :-- | :-- | :-- |
| 🥇 **대상** | KMR 빅데이터 센터 데이터 활용 아이디어 공모전 | `2023.12.13` | 중소기업 맞춤형 스마트팩토리 지표 · PCA + 군집화 (K-Means · GMM · 계층적 군집) |

<br/>

## 🎓 학력 & 📜 자격증

| 기간 | | |
| :-- | :-- | :-- |
| `2021.03 – 2026.02` | 🏫 **서울여자대학교** | 데이터사이언스학과 학사 |
| `2024.11` | 📊 **ADsP** | 데이터분석 준전문가 |
| `2025.04` | 🗄️ **SQLD** | SQL 개발자 |
| `2025.09 – 2026.03` | 🚀 **네이버 부스트캠프 AI Tech 8기** | NLP 트랙 |

<br/>

## 🛠 기술 스택

<div align="center">

<img src="https://skillicons.dev/icons?i=py,ts,js,pytorch,fastapi,nextjs,react&theme=dark" /><br/>
<img src="https://skillicons.dev/icons?i=postgres,cloudflare,vercel,docker,kubernetes,linux&theme=dark" /><br/>
<img src="https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square&logo=langchain&logoColor=white" /> <img src="https://img.shields.io/badge/Hugging_Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black" /> <img src="https://img.shields.io/badge/HyperCLOVA_X-03C75A?style=flat-square&logo=naver&logoColor=white" /> <img src="https://img.shields.io/badge/Claude_Code-D97757?style=flat-square&logo=anthropic&logoColor=white" />
<br/><br/>

**🕸️ 지식 그래프**<br/>
<img src="https://img.shields.io/badge/Neo4j-4581C3?style=for-the-badge&logo=neo4j&logoColor=white" /> <img src="https://img.shields.io/badge/Cypher-008CC1?style=for-the-badge&logo=neo4j&logoColor=white" /> <img src="https://img.shields.io/badge/Text2Cypher-6A1B9A?style=for-the-badge" /> <img src="https://img.shields.io/badge/GraphRAG-3E8E7E?style=for-the-badge" /> <img src="https://img.shields.io/badge/Graph_Modeling-193E45?style=for-the-badge" />

</div>

<br/>

<div align="center">
  <img src="https://streak-stats.demolab.com?user=alfks&theme=transparent&hide_border=true&ring=3E8E7E&fire=3E8E7E&currStreakLabel=3E8E7E&sideLabels=8B949E&dates=8B949E&stroke=30363D" />
</div>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:3E8E7E,100:193E45&height=100&section=footer" width="100%" />

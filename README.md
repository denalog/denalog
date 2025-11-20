<div align="center">


<svg width="900" height="420" viewBox="0 0 900 420" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <!-- 공통 네온 그라데이션 -->
    <linearGradient id="textGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#ff6ec7" />
      <stop offset="20%" stop-color="#f9ff6e" />
      <stop offset="40%" stop-color="#6effb5" />
      <stop offset="60%" stop-color="#6ea5ff" />
      <stop offset="80%" stop-color="#c56eff" />
      <stop offset="100%" stop-color="#ff6ec7" />
      <animate attributeName="x1" values="0%;100%;0%" dur="8s" repeatCount="indefinite" />
      <animate attributeName="x2" values="100%;200%;100%" dur="8s" repeatCount="indefinite" />
    </linearGradient>

    <!-- 공통 flicker 효과 -->
    <style>
      .flicker {
        animation: flicker 2.6s infinite ease-in-out;
      }
      @keyframes flicker {
        0%   { opacity: 1; }
        8%   { opacity: 0.85; }
        14%  { opacity: 0.6; }
        20%  { opacity: 1; }
        28%  { opacity: 0.75; }
        34%  { opacity: 1; }
        45%  { opacity: 0.9; }
        60%  { opacity: 1; }
        100% { opacity: 1; }
      }
    </style>

    <!-- Tech Stack 네온 보더 -->
    <linearGradient id="borderGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#ff6ec7">
        <animate attributeName="stop-color"
                 values="#ff6ec7; #f9ff6e; #6effb5; #6ea5ff; #c56eff; #ff6ec7"
                 dur="6s" repeatCount="indefinite" />
      </stop>
      <stop offset="100%" stop-color="#6effb5">
        <animate attributeName="stop-color"
                 values="#6effb5; #6ea5ff; #c56eff; #ff6ec7; #f9ff6e; #6effb5"
                 dur="6s" repeatCount="indefinite" />
      </stop>
    </linearGradient>

    <!-- 공통 네온 글로우 -->
    <filter id="neon">
      <feGaussianBlur stdDeviation="3" result="blur" />
      <feColorMatrix in="blur" type="matrix"
        values="0 0 0 0 1
                0 0 0 0 1
                0 0 0 0 1
                0 0 0 0.6 0" />
      <feMerge>
        <feMergeNode/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>
  </defs>

  <!-- 전체 배경 -->
  <rect x="0" y="0" width="900" height="420" fill="#040016"/>

  <!-- ==================== Welcome (테두리 없음) ==================== -->
  <g transform="translate(0, 0)">
    
    <!-- Welcome 텍스트만 -->
    <text x="60" y="90"
          class="flicker"
          font-family="Consolas, 'JetBrains Mono', 'Fira Code', monospace"
          font-size="40"
          fill="url(#textGrad)"
          filter="url(#neon)">
      Welcome!
    </text>

    <text x="60" y="135"
          class="flicker"
          font-family="Consolas, 'JetBrains Mono', 'Fira Code', monospace"
          font-size="22"
          fill="url(#textGrad)">
      This is Jena's GitHub space. Enjoy exploring my projects ✨
    </text>
  </g>

  <!-- ==================== Tech Stack Box ==================== -->
  <g transform="translate(0, 190)">
    <rect x="25" y="20" width="850" height="200" rx="18"
          fill="none" stroke="url(#borderGrad)" stroke-width="3" filter="url(#neon)"/>

    <rect x="35" y="30" width="830" height="180" rx="14"
          fill="#05001c" stroke="#1b1238" stroke-width="1"/>

    <!-- 픽셀 점 -->
    <circle cx="60" cy="60" r="3" fill="#ff6ec7" />
    <circle cx="75" cy="60" r="3" fill="#f9ff6e" />
    <circle cx="90" cy="60" r="3" fill="#6effb5" />
    <circle cx="105" cy="60" r="3" fill="#6ea5ff" />

    <text x="60" y="100"
          class="flicker"
          font-family="Consolas, 'JetBrains Mono', 'Fira Code', monospace"
          font-size="26"
          fill="url(#textGrad)"
          filter="url(#neon)">
      🧩 Tech Stack &amp; Interests
    </text>

    <text x="60" y="145"
          class="flicker"
          font-family="Consolas, 'JetBrains Mono', 'Fira Code', 'Noto Sans KR', monospace"
          font-size="18"
          fill="url(#textGrad)">
      🔭 요즘은 Next.js / Nuxt3 / TypeScript / AWS / LLM &amp; RAG 에 집중하고 있어요.
    </text>

    <text x="60" y="180"
          class="flicker"
          font-family="Consolas, 'JetBrains Mono', 'Fira Code', 'Noto Sans KR', monospace"
          font-size="18"
          fill="url(#textGrad)">
      🚀 애자일 프로세스 + 도메인 기반(DDD) 설계를 지키는 팀 개발을 선호합니다.
    </text>
  </g>
</svg>



---

### ⚡ Tech Stack

**Frontend**
- React, Next.js, Vue, Nuxt3  
- TypeScript, JavaScript, HTML, CSS, Tailwind, Vuetify

**Backend & API**
- Node.js, Express  
- Python, FastAPI, Django  
- REST API, JWT, Webhook, WebSocket

**Database & Infra**
- MySQL, PostgreSQL  
- AWS (S3, CloudFront, EC2, RDS, Route53, WAF)  
- Docker, Nginx

**DevOps & Collaboration**
- Git, GitHub Actions, Jenkins  
- Figma, Notion, Slack, Jira

**Currently Learning**
- LLM 기반 서비스 설계 (RAG, 벡터DB, Prompt Engineering)  
- 데이터 라벨링 파이프라인 및 모니터링 대시보드

---

### 💼 What I Do

- 서비스 **기획 → 설계 → 개발 → 배포**까지 전체 플로우를 직접 운영합니다.  
- 사용자 경험을 최우선으로 두고, 작은 인터랙션까지 세심하게 다듬는 걸 좋아해요.  
- 코드 구조와 협업 규칙(브랜치 전략, 커밋 컨벤션, 이슈 템플릿 등)을 설계해서  
  팀이 오래 유지되는 코드를 만들 수 있도록 돕습니다.

---

### 🌟 Featured Projects

- **HUNGLL** – LLM 기반 대화형 맞춤 맛집 추천 & 밥친구 매칭 서비스  
  → Nuxt3 + FastAPI + Django + RAG + AWS 인프라 설계 및 프론트엔드 리드

- **Smart Mattress Patient Monitoring Web App**  
  → Next.js + TypeScript 기반 실시간 모니터링 대시보드, 역할별(의사/간호사/보호자) UX 설계

- **Personal Tech Blog & Portfolio**  
  → Next.js 기반 GitHub 블로그, SEO와 페이지 구조까지 직접 설계 및 구현

> 위 프로젝트 부분은 실제 레포/서비스 링크로 교체해서 사용해 주세요 🙂

---

### 📊 GitHub Stats

<div align="center">

  <!-- GitHub Stats -->
  <img src="https://github-readme-stats.vercel.app/api?username=denalog&show_icons=true&theme=radical" height="165" />

  <!-- Top Languages -->
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=denalog&layout=compact&theme=radical" height="165" />

  <!-- Streak -->
  <img src="https://streak-stats.demolab.com?user=Ydenalog&theme=radical" height="165" />

</div>


### 💬 Contact & Links

- Email : higoonggi0906@gmail.com
- Portfolio / Blog : https://denalog.gihub.io

함께 이야기 나누거나 협업하고 싶다면 언제든 편하게 연락 주세요 🙌

### Featured Project — [Jenna's Portfolio](https://portfolio-pi-cyan-fzcirn5lpo.vercel.app)

BI Analyst 포트폴리오 사이트 · Next.js + Vercel로 직접 설계·구축

| 분류 | 기술 |
|------|------|
| Framework | Next.js 16 (App Router) |
| Language | TypeScript |
| Styling | Tailwind CSS v4 |
| Font | Pretendard · Manrope · Geist Mono |
| Deploy | Vercel (git push → 자동 배포) |

**Architecture**
- CMS / DB 없이 \src/lib/projects.ts\ 단일 파일이 모든 콘텐츠의 source of truth
- 각 프로젝트는 섹션 배열(\cards\ \kpis\ \par\ \lessons\ 등)로 구성되며, \kind\ 필드로 컴포넌트를 선택해 렌더링
- \generateStaticParams\로 빌드 시 정적 생성(SSG) → Vercel 자동 배포

**의사결정**
- CMS 도입 대신 TS 파일 직접 편집 선택 → 1인 운영 환경에서 관리 오버헤드 최소화
- **Claude Code** 와 자연어 대화로 파일 편집 + git commit까지 처리하는 zero-friction workflow 구성

**트러블슈팅**
- \git pull --rebase\ 중 PowerShell 기본 인코딩으로 한글 깨짐 → \WriteAllText\ + UTF-8 명시로 해결

---

### Job Search Automation Pipeline

Node.js + Playwright 기반 채용공고 자동 수집 · 분류 · 리포트 발행 시스템

| | |
|---|---|
| 크롤링 | Playwright stealth — 원티드 · 사람인 · 잡코리아 · 리멤버 |
| 스코어링 | BI/Analytics 키워드 가중치 기반 ★★★ / ★★ / ★ 자동 분류 |
| 스케줄 | GitHub Actions cron — 매일 오전 9시 KST 자동 실행 |
| 출력 | HTML 리포트 생성 → GitHub Pages 배포 |

→ [최신 리포트 보기](https://dearkimm.github.io/Portfolio/job-search/job-report.html)

---

<div align=center>

[![Portfolio Badge](http://img.shields.io/badge/-Portfolio-black?style=flat-square&logo=vercel&logoColor=white&link=https://portfolio-pi-cyan-fzcirn5lpo.vercel.app)](https://portfolio-pi-cyan-fzcirn5lpo.vercel.app)
[![LinkedIn Badge](https://img.shields.io/badge/-LinkedIn-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/%EA%B9%80%EC%A0%95%EB%AF%BCjenna)](https://www.linkedin.com/in/%EA%B9%80%EC%A0%95%EB%AF%BCjenna)
[![Gmail Badge](https://img.shields.io/badge/-Gmail-d14836?style=flat-square&logo=Gmail&logoColor=white&link=mailto:dearkimm@sookmyung.ac.kr)](mailto:dearkimm@sookmyung.ac.kr)

</div>

[![gitanimals](https://render.gitanimals.org/farms/Dearkimm)](https://github.com/devxb/gitanimals)

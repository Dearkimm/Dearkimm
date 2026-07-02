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
- 별도 CMS나 데이터베이스 없이, 모든 프로젝트 콘텐츠를 파일 하나(`src/lib/projects.ts`)에서 관리
- 프로젝트마다 "소개 카드 / 성과 지표 / 문제해결 과정" 같은 섹션을 데이터로 정의해두면, 화면에서는 그 데이터를 읽어 알맞은 컴포넌트를 자동으로 골라 렌더링
- 빌드 시점에 모든 페이지를 미리 정적 HTML로 만들어두는 방식(SSG)이라, 방문자가 접속하면 서버 처리 없이 즉시 로딩되고 Vercel이 push마다 자동 배포

**의사결정**
- CMS 도입 대신 TS 파일 직접 편집 선택 → 1인 운영 환경에서 관리 오버헤드 최소화
- **Claude Code** 와 자연어 대화로 파일 편집 + git commit까지 처리하는 zero-friction workflow 구성

---

### Job Search Automation Pipeline

Node.js + Playwright 기반 채용공고 자동 수집 · 분류 · 리포트 발행 시스템

| | |
|---|---|
| 크롤링 | Playwright stealth — 원티드 · 사람인 · 잡코리아 · 리멤버 |
| 스코어링 | BI/Analytics 키워드 가중치 기반 ★★★ / ★★ / ★ 자동 분류 |
| 스케줄 | GitHub Actions cron — 매일 오전 9시 KST 자동 실행 |
| 출력 | HTML 리포트 생성 → Vercel 배포 (`public/`에 저장되어 포트폴리오 사이트와 함께 서빙) |

→ [최신 리포트 보기](https://portfolio-pi-cyan-fzcirn5lpo.vercel.app/job-search/job-report.html)

---

<div align=center>

[![Portfolio Badge](http://img.shields.io/badge/-Portfolio-black?style=flat-square&logo=vercel&logoColor=white&link=https://portfolio-pi-cyan-fzcirn5lpo.vercel.app)](https://portfolio-pi-cyan-fzcirn5lpo.vercel.app)
[![LinkedIn Badge](https://img.shields.io/badge/-LinkedIn-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/%EA%B9%80%EC%A0%95%EB%AF%BCjenna)](https://www.linkedin.com/in/%EA%B9%80%EC%A0%95%EB%AF%BCjenna)
[![Gmail Badge](https://img.shields.io/badge/-Gmail-d14836?style=flat-square&logo=Gmail&logoColor=white&link=mailto:dearkimm@sookmyung.ac.kr)](mailto:dearkimm@sookmyung.ac.kr)

</div>

[![gitanimals](https://render.gitanimals.org/farms/Dearkimm)](https://github.com/devxb/gitanimals)

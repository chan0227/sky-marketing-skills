# Sky AI Marketing Skills 🇰🇷

> **한국 시장에 최적화된 AI 마케팅 스킬팩**
> Corey Haines의 [marketingskills](https://github.com/coreyhaines31/marketingskills) (28.6k ⭐) 기반 — 한국형 확장 버전

[![Original](https://img.shields.io/badge/Forked%20from-coreyhaines31%2Fmarketingskills-blue)](https://github.com/coreyhaines31/marketingskills)
[![Made by](https://img.shields.io/badge/Made%20by-Sky%20AI-orange)](https://sky-ai.kr)
[![Purpose](https://img.shields.io/badge/Purpose-Education%20%26%20Demo-green)](#-교육-시연-가이드)

---

## 🎯 이 프로젝트가 뭔가요?

**Sky AI Marketing Skills**는 글로벌에서 검증된 마케팅 스킬 시스템을 **한국 비즈니스 환경에 맞춰 재해석한 교육용 오픈소스**입니다.

원본은 영어권 SaaS·B2B 마케팅 맥락이라 한국 기업이 그대로 쓰기엔 어색했습니다. 그래서 **5개 한국 특화 스킬을 추가**하고, AI 교육 강의에서 **라이브 시연이 가능한 형태**로 재구성했습니다.

### 누구를 위한 것인가요?

- 🏢 **기업 AI 교육 담당자** — Claude/ChatGPT 실무 활용을 가르치시는 분
- 🏛️ **공공기관 디지털 혁신 담당자** — 정부·지자체에서 생성형 AI 도입하시는 분
- 📚 **AI 강사·컨설턴트** — 강의 시연용 실전 사례가 필요한 분
- 🚀 **한국 기반 마케터·기획자** — Claude Code로 실무 자동화하시는 분

---

## ✨ 한국형 5대 추가 스킬

| 스킬명 | 한 줄 설명 | 주요 사용 사례 |
|---|---|---|
| 🔍 [`korean-seo`](./skills/korean-seo) | 네이버·카카오·구글 한국 검색 최적화 | 블로그 상위노출, 지식iN 활용, 카페 마케팅 |
| 🏛️ [`korea-b2g-sales`](./skills/korea-b2g-sales) | 한국 B2B/공공 영업 자료 자동 생성 | 정부 제안서, 공공기관 영업, 입찰 대응 |
| ✍️ [`korean-content-marketing`](./skills/korean-content-marketing) | 한국형 콘텐츠 마케팅 | 티스토리·네이버 블로그, 인스타, 브런치 |
| 📊 [`korean-ad-performance`](./skills/korean-ad-performance) | 한국 광고 플랫폼 퍼포먼스 마케팅 | 네이버GFA, 카카오모먼트, 메타광고 한국 최적화 |
| 🎓 [`ai-education-marketing`](./skills/ai-education-marketing) | AI 교육 사업 마케팅 (Sky AI 전용) | 기업 교육 영업, 공공 교육 수주, 강사 브랜딩 |

원본 32개 스킬(CRO, copywriting, ai-seo 등)도 그대로 포함되어 있어 **총 37개 스킬**을 활용하실 수 있습니다.

---

## 🚀 빠른 시작 (3가지 방법)

### 방법 1: Claude Code 플러그인 ⭐ (가장 쉬움)

```bash
# Claude Code 안에서 실행
/plugin marketplace add [your-github-id]/sky-marketing-skills
/plugin install sky-marketing-skills
```

### 방법 2: npx로 특정 스킬만

```bash
# 한국형 스킬 5개만 설치
npx skills add [chan0227]/sky-marketing-skills --skill korean-seo korea-b2g-sales korean-content-marketing korean-ad-performance ai-education-marketing
```

### 방법 3: 직접 클론 (커스터마이징용)

```bash
git clone https://github.com/[your-github-id]/sky-marketing-skills.git
cp -r sky-marketing-skills/skills/* .claude/skills/
```

---

## 🎬 교육·시연 가이드

이 저장소는 **AI 교육 강의에서 실시간 시연**을 염두에 두고 설계되었습니다.

### 강의 시연 시나리오 3종

📁 [`docs/demo-scenarios.md`](./docs/demo-scenarios.md)에 한국은행, 제일기획, 공공기관 교육에서 바로 쓸 수 있는 **30분짜리 라이브 데모 스크립트**가 들어있습니다.

| 시나리오 | 대상 | 시연 시간 | 사용 스킬 |
|---|---|---|---|
| **시나리오 A**: "팀장이 신규 사업 보고서 한 장 만들라고 했다" | 한국은행·금융권 팀장급 | 25분 | `korea-b2g-sales` + `copywriting` |
| **시나리오 B**: "광고대행사 신입이 캠페인 기획서 첫 작성" | 제일기획·광고대행사 신입 | 30분 | `korean-ad-performance` + `ad-creative` |
| **시나리오 C**: "공공기관에서 정책 홍보 콘텐츠 제작" | 공무원·공공기관 직원 | 20분 | `korean-content-marketing` + `korean-seo` |

### 강의에서 강조하는 3가지 메시지

1. **"AI는 도구가 아니라 동료다"** — 스킬 시스템을 통해 AI에게 회사 맥락을 학습시키는 과정 시연
2. **"한 번 만들면 평생 자산"** — fork → 커스터마이징 → 팀 전체 공유의 가치
3. **"글로벌 표준 + 한국 현지화"** — 28.6k ⭐ 글로벌 자산을 자기 비즈니스로 만드는 방법

---

## 📊 원본 vs Sky AI 한국판

| 항목 | 원본 (coreyhaines31) | Sky AI 한국판 |
|---|---|---|
| 스킬 수 | 32개 | **37개** (+5개 한국 특화) |
| 언어 | 영어 | 한국어 + 영어 병기 |
| 시장 맥락 | 미국 SaaS/B2B | 한국 B2B/B2G/B2C 전반 |
| 광고 플랫폼 | Google, Meta | + **네이버GFA, 카카오모먼트** |
| SEO 대상 | 구글 | + **네이버, 다음, 지식iN, 카페** |
| 영업 자료 | 미국식 sales deck | + **한국 정부 제안서, 공공 입찰** |
| 교육 자료 | 일반 마케터용 | + **AI 교육 강사·컨설턴트용** |

상세 차이점: [`docs/MIGRATION.md`](./docs/MIGRATION.md)

---

## 🏗️ 폴더 구조

```
sky-marketing-skills/
├── README.md                          # 지금 보고 계신 이 파일
├── .claude-plugin/                    # Claude Code 플러그인 매니페스트
│   └── marketplace.json
├── skills/                            # 핵심 스킬 모음
│   ├── korean-seo/                    # 🆕 한국형 추가
│   ├── korea-b2g-sales/               # 🆕 한국형 추가
│   ├── korean-content-marketing/      # 🆕 한국형 추가
│   ├── korean-ad-performance/         # 🆕 한국형 추가
│   ├── ai-education-marketing/        # 🆕 한국형 추가
│   ├── cro/                           # 원본 유지
│   ├── copywriting/                   # 원본 유지
│   ├── ai-seo/                        # 원본 유지
│   └── ... (29개 원본 스킬)
├── docs/                              # 🆕 한국어 가이드
│   ├── demo-scenarios.md              # 강의 시연 시나리오
│   ├── MIGRATION.md                   # 원본과의 차이점
│   └── KOREAN-MARKETING-CONTEXT.md    # 한국 마케팅 환경 가이드
└── tools/                             # 원본 CLI 도구
```

---

## 🤝 기여하기

이 저장소는 **GPTers AI 스터디 그룹**과 한국 AI 커뮤니티의 자산을 목표로 합니다.

기여 방법:
1. 이 저장소를 fork → 자기 스킬 추가
2. Pull Request 보내주시면 검토 후 병합
3. Issue로 새 스킬 제안 가능

특히 이런 분들의 PR을 환영합니다:
- 🏛️ 지자체 마케팅·홍보 담당 공무원
- 📱 한국 광고대행사 AE/플래너
- 🎓 AI 강사·교육 컨설턴트
- ✍️ 한국 콘텐츠 마케터

---

## 📜 라이선스 & 출처

- **원본**: [coreyhaines31/marketingskills](https://github.com/coreyhaines31/marketingskills) by Corey Haines (MIT License)
- **한국판 확장**: Sky AI (MIT License)
- **상업적 사용**: 가능 (라이선스 명시 필수)

---

## 📞 문의

- **Sky AI**: cdragon0227@gmail.com
- **GPTers AI 스터디 그룹** 21기 멤버 우선 안내
- **이슈/문의**: GitHub Issues 활용

> *"AI 교육은 단순 도구 사용법이 아니라, 자기 비즈니스의 자산으로 만드는 방법을 가르치는 것입니다."*
> — Sky AI 부사장 성찬용

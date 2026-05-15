# 📊 MIGRATION.md — 원본 vs Sky AI 한국판 차이점

> 이 문서는 [coreyhaines31/marketingskills](https://github.com/coreyhaines31/marketingskills) 원본과 Sky AI 한국판의 차이점을 정리합니다.
> 원본을 알고 계신 분, 또는 영문권 마케팅 컨텍스트와 한국 마케팅 컨텍스트의 차이를 학습하시려는 분에게 유용합니다.

---

## 1. 핵심 철학의 차이

| 구분 | 원본 (Corey Haines) | Sky AI 한국판 |
|---|---|---|
| 주 대상 | 미국 SaaS 창업자·테크 마케터 | 한국 기업·공공기관·AI 강사 |
| 시장 가정 | 자유시장 B2B SaaS | B2B + B2G 혼합 (공공조달 비중 큼) |
| 영업 사이클 | 짧음 (수주~수개월) | 김 (수개월~1년+) |
| 의사결정 구조 | 빠른 단일 의사결정자 | 다단계 결재·관계 중시 |
| 콘텐츠 채널 | 구글·LinkedIn·X 중심 | 네이버·카카오·인스타 중심 |
| 광고 플랫폼 | Google Ads·Meta 중심 | 네이버GFA·카카오모먼트 추가 |

---

## 2. 5대 한국 특화 스킬 신규 추가

### 추가 스킬 vs 원본 유사 스킬

| 신규 스킬 | 원본 유사 스킬 | 핵심 차이 |
|---|---|---|
| `korean-seo` | `ai-seo`, `seo-audit` | C-Rank/D.I.A 알고리즘, 네이버 채널 전략 추가 |
| `korea-b2g-sales` | `sales-enablement` | 한국 공공조달, RFP 응답, 결재 문화 반영 |
| `korean-content-marketing` | `copywriting` | 네이버 블로그·티스토리·브런치·카카오 채널 추가 |
| `korean-ad-performance` | `ad-creative` | 네이버 GFA, 카카오모먼트 등 한국 플랫폼 추가 |
| `ai-education-marketing` | (없음) | Sky AI 사업 영역 특화, 완전 신규 |

### 왜 단순 번역이 아닌 신규 스킬로 만들었나?

영문 → 한글 번역만으로는 다음 한계가 있습니다:

1. **알고리즘 자체가 다름** — 네이버 C-Rank는 구글 PageRank와 작동 원리가 다름
2. **소비자 행동이 다름** — 한국인은 "지식iN" 같은 Q&A 플랫폼 의존도가 매우 높음
3. **B2B 문화가 다름** — 한국은 관계·절차·양식 중시, 미국은 가치·속도 중시
4. **광고 플랫폼이 다름** — 네이버·카카오는 글로벌 어디에도 없음
5. **공공 영업이 거대 시장** — 미국 마케팅 스킬은 B2G를 거의 다루지 않음

---

## 3. 원본 32개 스킬 유지 + 보조 활용 권장

원본 스킬은 **그대로 유지**하며, 한국 시장에서는 보조적으로 활용합니다:

| 원본 스킬 | 한국 시장 활용도 | 활용 권장 상황 |
|---|---|---|
| `cro` | ⭐⭐⭐⭐ | 한국 이커머스·랜딩페이지에도 적용 가능 |
| `copywriting` | ⭐⭐⭐ | 영문 카피·해외 진출 시 |
| `ai-seo` | ⭐⭐⭐⭐ | 구글·AI 검색 (네이버는 `korean-seo`) |
| `seo-audit` | ⭐⭐⭐ | 구글 SEO 진단 시 |
| `analytics` | ⭐⭐⭐⭐⭐ | GA4 등 글로벌 동일 |
| `emails` | ⭐⭐⭐⭐ | 이메일 마케팅 글로벌 공통 |
| `ad-creative` | ⭐⭐⭐ | 메타·구글 광고 (네이버·카카오는 `korean-ad-performance`) |
| `sales-enablement` | ⭐⭐⭐ | 외국계·B2B SaaS (공공은 `korea-b2g-sales`) |
| `revops` | ⭐⭐⭐⭐ | 영업 운영 글로벌 동일 |
| `churn-prevention` | ⭐⭐⭐⭐ | 구독 모델 글로벌 공통 |
| `lead-magnets` | ⭐⭐⭐⭐ | 한국 시장에도 적용 가능 |
| `site-architecture` | ⭐⭐⭐⭐⭐ | 글로벌 공통 |

**활용 원칙**: 한국 특화 스킬 5개를 **메인**으로, 원본 스킬을 **보조**로 사용.

---

## 4. 폴더 구조 차이

### 원본 구조
```
marketingskills/
├── .claude-plugin/
├── .github/
├── skills/                    # 32개
├── tools/
├── AGENTS.md
├── CLAUDE.md
├── README.md                  # 영문
└── VERSIONS.md
```

### Sky AI 한국판 구조
```
sky-marketing-skills/
├── .claude-plugin/
├── .github/
├── skills/                    # 32개 (원본) + 5개 (한국 특화) = 37개
│   ├── korean-seo/            # 🆕
│   ├── korea-b2g-sales/       # 🆕
│   ├── korean-content-marketing/  # 🆕
│   ├── korean-ad-performance/ # 🆕
│   └── ai-education-marketing/    # 🆕
├── tools/
├── docs/                      # 🆕 한국어 가이드
│   ├── demo-scenarios.md      # 강의 시연 시나리오
│   ├── MIGRATION.md           # 이 파일
│   └── KOREAN-MARKETING-CONTEXT.md  # 한국 마케팅 환경 가이드
├── AGENTS.md
├── CLAUDE.md
├── README.md                  # 한국어 (영문 출처 명시)
└── VERSIONS.md
```

---

## 5. 라이선스 & 출처 명시

### 라이선스
- **원본**: MIT License (Corey Haines)
- **Sky AI 한국판**: MIT License (Sky AI)

### 출처 표기 의무
모든 사용자는 다음을 README 또는 LICENSE 파일에 명시해야 합니다:

```
This project is based on coreyhaines31/marketingskills (MIT License)
with Korean market adaptations by Sky AI (MIT License).
```

### Fork 시 권장 사항
- ✅ 이 저장소를 fork → 자기 비즈니스에 맞춰 추가 커스터마이징
- ✅ 자기 회사·기관 특화 스킬을 추가 (예: `samsung-sales`, `lg-content`)
- ✅ 개선 사항은 PR로 기여 (Sky AI 또는 원본에)
- ❌ 원본 출처 삭제 후 재배포

---

## 6. 업데이트 정책

### 원본 업데이트 추적
- 원본이 업데이트되면 Sky AI 한국판도 **월 1회** 동기화
- 동기화 일정: 매월 15일경
- 동기화 내역은 `VERSIONS.md`에 기록

### 한국 시장 변화 반영
- 한국 검색·광고 플랫폼 정책 변경 시 즉시 반영
- 정부 사업 정책 변화 시 `korea-b2g-sales` 업데이트
- 한국 AI 정책 변화 시 `ai-education-marketing` 업데이트

---

## 7. 향후 추가 예정 스킬 (로드맵)

다음 한국 특화 스킬을 추가 고려 중:

| 후보 스킬 | 우선순위 | 예상 시기 |
|---|---|---|
| `korean-pr-media` (한국 언론·PR) | 높음 | Q3 2026 |
| `korean-ecommerce-conversion` (네이버·쿠팡 전환 최적화) | 높음 | Q3 2026 |
| `korean-b2c-customer-journey` (한국 소비자 여정) | 중간 | Q4 2026 |
| `korean-startup-fundraising` (한국 스타트업 IR) | 중간 | Q4 2026 |
| `korean-influencer-marketing` (한국 인플루언서 마케팅) | 중간 | 2027 |

**제안 환영**: GitHub Issues로 신규 스킬 아이디어 제안 가능.

---

## 8. 사용 사례 (Use Cases)

이 패키지가 실제로 적용된 사례:

### 기업 사례
- 한국은행 임원·팀장 대상 AI 활용 교육 (5개 모듈)
- 제일기획 신입사원 Claude Cowork 교육
- 한국기술대학교 RISE사업단 청소년 AI 창업 교육

### 공공 사례
- 아산시청 공무원 AI 교육 제안서
- 충남 자치경찰 AI 교육 기획
- 정부 부처 AI 정책 교육 자료

### 교육 사례
- GPTers AI 스터디 그룹 21기 콘텐츠
- 서울대 AI 세미나 (2025년 10월)

---

## 9. 자주 묻는 질문

**Q1: 영문 원본 스킬도 한국에서 쓸 만한가요?**
> A: 네. `analytics`, `revops`, `lead-magnets`, `churn-prevention` 등은 한국에서도 효과적입니다. 다만 `copywriting`, `seo`, `sales`, `ad-creative`는 한국 특화 버전을 권장합니다.

**Q2: 원본을 두고 왜 Sky AI 버전을 써야 하나요?**
> A: 한국 시장에서는 네이버·카카오 같은 글로벌에 없는 플랫폼이 시장의 70%+를 차지합니다. 원본만으로는 이 영역을 다룰 수 없습니다.

**Q3: 두 저장소를 동시에 쓸 수 있나요?**
> A: 가능하지만 권장하지 않습니다. Sky AI 버전이 원본을 모두 포함하므로 한쪽만 쓰시면 됩니다. 단, 원본의 최신 스킬은 동기화 전까지 지연이 있을 수 있습니다.

**Q4: 기관·회사용으로 추가 커스터마이징하려면?**
> A: 이 저장소를 fork → 자기 조직 스킬 추가 → 내부 사용. Sky AI에 컨설팅 의뢰 시 12주 안에 조직 맞춤 스킬 20~30개 구축 가능.

---

## 10. 기여자 (Contributors)

- **원본 저자**: [Corey Haines](https://github.com/coreyhaines31) (28.6k ⭐ marketingskills)
- **한국판 책임자**: 성찬용 (Sky AI 부사장)
- **검토·자문**: GPTers AI 스터디 그룹 21기

기여를 환영합니다. CONTRIBUTING.md를 참고해주세요.

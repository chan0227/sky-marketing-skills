# 🚀 Fork & 적용 가이드 (부사장님 전용)

> 이 문서는 부사장님께서 **GitHub에서 fork한 후**, 제가 만들어드린 Sky AI 한국판 콘텐츠를 적용하는 단계별 절차입니다.

---

## ⚡ 빠른 실행 순서 (총 30분)

### Step 1: GitHub에서 Fork (5분)

1. https://github.com/coreyhaines31/marketingskills 접속
2. 우측 상단 **"Fork"** 버튼 클릭
3. 다음과 같이 입력:
   - **Owner**: 부사장님 GitHub 계정
   - **Repository name**: `sky-marketing-skills` (또는 원하는 이름)
   - **Description**: `한국 시장에 최적화된 AI 마케팅 스킬팩 | Forked from coreyhaines31/marketingskills | Sky AI Education`
   - ✅ **"Copy the main branch only"** 체크
4. **"Create fork"** 클릭
5. 약 10초 후 `https://github.com/[부사장님계정]/sky-marketing-skills`로 이동됨

### Step 2: 로컬에 클론 (3분)

부사장님 작업 PC에서 터미널 열고:

```bash
# 1. 원하는 폴더로 이동 (예: ~/projects)
cd ~/projects

# 2. fork한 저장소 클론 ([부사장님계정] 부분만 본인 ID로 변경)
git clone https://github.com/[부사장님계정]/sky-marketing-skills.git

# 3. 클론된 폴더로 이동
cd sky-marketing-skills
```

### Step 3: 제가 만들어드린 파일 적용 (10분)

부사장님 PC에 있는 클론된 폴더로, 제가 `/home/claude/sky-marketing-skills/`에 만든 파일들을 복사합니다.

**방법 A: 한 번에 다운로드 후 복사 (권장)**

이 대화 마지막에 제가 `present_files`로 압축 파일을 만들어드릴 예정입니다. 그 파일을 다운로드 받으신 후:

```bash
# 다운로드 받은 압축 파일 압축 해제
unzip ~/Downloads/sky-marketing-skills-korean-pack.zip -d ~/temp-sky-pack

# fork한 저장소에 복사
cp -r ~/temp-sky-pack/* ~/projects/sky-marketing-skills/

# 작업 폴더로 이동
cd ~/projects/sky-marketing-skills
```

**방법 B: 파일 하나씩 수동 복사**

위 방법이 어려우시면, 각 파일 내용을 복사해서 다음 위치에 붙여넣기:

```
sky-marketing-skills/
├── README.md (덮어쓰기)
├── .claude-plugin/marketplace.json (덮어쓰기)
├── skills/
│   ├── korean-seo/SKILL.md (신규)
│   ├── korea-b2g-sales/SKILL.md (신규)
│   ├── korean-content-marketing/SKILL.md (신규)
│   ├── korean-ad-performance/SKILL.md (신규)
│   └── ai-education-marketing/SKILL.md (신규)
└── docs/
    ├── demo-scenarios.md (신규)
    └── MIGRATION.md (신규)
```

### Step 4: README의 [your-github-id] 부분 수정 (2분)

```bash
# 부사장님 GitHub ID로 일괄 치환 (예: cdragon0227)
sed -i '' 's/\[your-github-id\]/cdragon0227/g' README.md
sed -i '' 's/\[your-id\]/cdragon0227/g' .claude-plugin/marketplace.json

# Linux/WSL이면:
# sed -i 's/\[your-github-id\]/cdragon0227/g' README.md
# sed -i 's/\[your-id\]/cdragon0227/g' .claude-plugin/marketplace.json
```

### Step 5: Git 커밋 & 푸시 (5분)

```bash
# 변경사항 확인
git status

# 모든 변경사항 추가
git add .

# 커밋
git commit -m "feat: Add Korean market adaptation (5 skills + docs)

- Add 5 Korea-specific skills:
  * korean-seo (네이버/카카오/구글 한국 SEO)
  * korea-b2g-sales (한국 B2B/B2G 영업)
  * korean-content-marketing (한국 콘텐츠 마케팅)
  * korean-ad-performance (네이버GFA, 카카오모먼트 광고)
  * ai-education-marketing (AI 교육 마케팅, Sky AI 전용)
- Add Korean README.md (한국어 가이드)
- Add demo scenarios for AI education classes
- Add MIGRATION.md (원본 vs 한국판 차이점)
- Update marketplace.json with Korean skills

Based on coreyhaines31/marketingskills v2.0.0 (MIT License)
Korean adaptation by Sky AI"

# GitHub로 푸시
git push origin main
```

### Step 6: GitHub에서 확인 (3분)

1. `https://github.com/[부사장님계정]/sky-marketing-skills` 새로고침
2. README.md가 한국어로 표시되는지 확인
3. `skills/` 폴더에 5개 한국 특화 폴더가 있는지 확인
4. `docs/` 폴더가 새로 생긴 것 확인

### Step 7: Topics 태그 추가 (2분, GitHub 웹에서)

저장소 페이지에서 우측 상단 ⚙️ 아이콘 → "Topics" 추가:
- `korean-marketing`
- `claude-code`
- `ai-skills`
- `b2g-sales`
- `naver-seo`
- `kakao-marketing`
- `ai-education`
- `sky-ai`

→ GitHub 검색에서 한국 마케터들이 찾기 쉬워집니다.

---

## 🎯 Fork 완료 후 즉시 할 수 있는 것

### ✅ 1. 강의에서 라이브 시연
- GitHub URL을 강의 화면에 띄우고 "이게 글로벌 28.6k ⭐ 기반 한국형 패키지"라고 소개
- `docs/demo-scenarios.md`의 시나리오를 그대로 실행

### ✅ 2. 영업 자료에 추가
- Sky AI 회사 소개서·제안서에 "Sky AI는 글로벌 자산을 한국화하여 오픈소스로 기여" 항목 추가
- 신뢰도·전문성 증거로 활용

### ✅ 3. GPTers 커뮤니티 공유
- GPTers 21기 슬랙/디스코드에 GitHub URL 공유
- "한국 AI 마케팅 스킬 오픈소스 만들었습니다" 소개글

### ✅ 4. Claude Code에서 직접 사용
```bash
# 부사장님 PC의 Claude Code에서
/plugin marketplace add [부사장님계정]/sky-marketing-skills
/plugin install sky-marketing-skills
```

---

## 🔄 향후 유지·발전 가이드

### 월 1회 동기화 (원본 업데이트 추적)

```bash
cd ~/projects/sky-marketing-skills

# 원본 저장소를 upstream으로 추가 (처음 한 번만)
git remote add upstream https://github.com/coreyhaines31/marketingskills.git

# 원본 최신 변경사항 가져오기 (월 1회)
git fetch upstream
git merge upstream/main

# 충돌 해결 후 푸시
git push origin main
```

### 신규 한국 스킬 추가 시

```bash
# 새 스킬 폴더 생성
mkdir -p skills/korean-pr-media

# SKILL.md 작성 (다른 스킬 참고)
nano skills/korean-pr-media/SKILL.md

# marketplace.json에 추가
nano .claude-plugin/marketplace.json

# 커밋 & 푸시
git add .
git commit -m "feat: Add korean-pr-media skill"
git push
```

### 다른 사람의 기여(PR) 받는 법

1. GitHub에서 Pull Request 알림 확인
2. 코드 검토 (Files Changed 탭)
3. 문제없으면 "Merge pull request" 클릭
4. CONTRIBUTORS.md에 기여자 추가

---

## 💡 부사장님께 추가 제안

### 제안 1: 영상 콘텐츠 제작
- GitHub 저장소 소개 영상 5분 (YouTube 쇼츠)
- "글로벌 28.6k ⭐ 자산을 어떻게 자기 비즈니스로 만드는가" 스토리

### 제안 2: 블로그 시리즈
- `tistory-blog-writer` 스킬로 5편 시리즈 자동 작성:
  - 1편: "글로벌 마케팅 스킬을 한국화하다"
  - 2편: "네이버 SEO 스킬 만들기"
  - 3편: "한국 B2G 영업 스킬 만들기"
  - 4편: "AI 강사가 AI 도구를 만드는 이유"
  - 5편: "오픈소스 기여로 비즈니스 키우기"

### 제안 3: 강사 양성 과정 콘텐츠
- 이 fork 프로젝트 자체를 **"AI 강사 양성 과정"의 실습 프로젝트**로 활용
- 수강생이 자기 분야 스킬을 fork & 추가 → 포트폴리오

### 제안 4: 정부 사업 활용
- "한국 AI 마케팅 스킬 오픈소스 생태계 구축" 명목으로 정부 사업 신청 가능
- 과기부·정보통신산업진흥원(NIPA) 디지털 인재 양성 사업 등

---

## ❓ 자주 묻는 질문

**Q1: Fork만 하고 안 쓰면 무슨 일이 생기나요?**
> A: 아무 일도 안 생깁니다. 부사장님 계정에 사본만 남습니다. 부담 없이 진행하세요.

**Q2: 나중에 fork를 삭제하고 싶으면?**
> A: GitHub 저장소 페이지 → Settings → 맨 아래 "Delete this repository" → 저장소 이름 입력하면 삭제. 원본에는 영향 없습니다.

**Q3: Private으로 바꿀 수 있나요?**
> A: 가능합니다. Settings → "Change repository visibility" → "Make private". 단, 강의 시연용이라 Public 권장.

**Q4: 누가 무단 복사하면 어떡하나요?**
> A: MIT 라이선스라 자유 복사 가능합니다. 단, "Sky AI 기반" 출처는 명시해야 합니다 (라이선스 조건).

**Q5: 한국어 번역에 오류가 있으면?**
> A: 부사장님이 직접 수정 후 커밋하시거나, GitHub Issues로 받으시면 됩니다.

---

## 📞 막히시면

이 가이드대로 진행하시다가 막히는 부분이 있으면, 다음 정보와 함께 말씀해주세요:

1. 어느 Step에서 막혔는지
2. 실행한 명령어
3. 화면에 표시된 에러 메시지

제가 다음 단계를 도와드리겠습니다.

---

**예상 완료 시각**: 부사장님이 지금 시작하시면 **30분 후 GitHub에 Sky AI Marketing Skills v1.0.0이 공개**되어 있을 것입니다. 🚀

# 데우스 원정대 (Deus Expedition)

웹소설을 비주얼 노벨 게임으로 변환하는 프로젝트입니다.

## 프로젝트 개요

- **총 편수**: 180편 (확장 시 최대 200편)
- **1편 분량**: 약 4,000자 (공백 포함)
- **총 분량**: 약 130~150권 (웹소설 기준)
- **구조**: 3막 → 각 막을 여러 챕터로 → 각 챕터를 여러 편으로

## 디렉토리 구조

```
deus-expedition/
├── README.md                    # 이 파일
├── WRITING_GUIDE.md            # 대본 작성 가이드 (필독!)
├── EPISODE_TEMPLATE.md         # 에피소드 템플릿
├── Characters.md               # 캐릭터 설정
├── Worldbuilding.md           # 세계관 설정
├── Style.md                   # 문체 가이드
├── Genre.md                   # 장르 정의
├── Braindump.md              # 핵심 아이디어
├── Outline/                   # 전체 구조 및 챕터별 아웃라인
│   ├── full-structure.md     # 180편 전체 구조 (필독!)
│   ├── outline-chapter-1.md  # 챕터 1 아웃라인
│   └── ...
├── Chapters/                  # 완성된 에피소드 대본
│   ├── episode-2-1.md        # 예시 에피소드
│   └── ...
├── Archive/                   # 보관 자료
├── Assets/                    # 리소스 목록
└── Research/                  # 리서치 자료
```

## 시작하기

### 1. 필수 문서 읽기 (순서대로)

1. **README.md** (이 파일) - 프로젝트 개요
2. **Braindump.md** - 핵심 아이디어와 테마
3. **Outline/full-structure.md** - 180편 전체 구조
4. **Characters.md** - 캐릭터 설정
5. **Worldbuilding.md** - 세계관 설정
6. **Style.md** - 문체 가이드
7. **WRITING_GUIDE.md** - 대본 작성 가이드 ⭐ 가장 중요!

### 2. 에피소드 작성하기

1. `Outline/full-structure.md`에서 작성할 에피소드 확인
2. `EPISODE_TEMPLATE.md`를 복사하여 새 파일 생성
3. `WRITING_GUIDE.md`를 참고하여 작성
4. `Chapters/episode-X-Y.md` 형식으로 저장
5. Git commit & push

### 3. 예시 참고

- **1-1 대본**: `1-1 대본.docx` (원본 참고용)
- **2-1 에피소드**: `Chapters/episode-2-1.md` (완성 예시)

## 작성 규칙

### 형식
- `·` 기호로 시작하는 대사/독백 형식
- `· (독백)` - A의 1인칭 독백
- `· 캐릭터명: "대사"` - 캐릭터 대사
- `[ 리듬 게임 진입 ]` - 게임플레이 요소 표시

### 분량
- **1편당 약 4,000자** (공백 포함)
- 대사는 2-3줄까지 허용

### 스타일
- 거칠고 직설적인 A의 목소리
- 냉소적이면서도 예리한 관찰
- 간결한 문장, 감각적 묘사
- 비속어 사용 가능 ("빌어먹을", "젠장" 등)

### 리소스 정리
- 각 에피소드 끝에 **리소스 정리 섹션** 필수
- 배경 이미지, 캐릭터 스프라이트, CG, 음악, 효과음 목록
- 신규/재사용 여부 표시

## 브랜치 전략

- `main` - 완성된 에피소드만
- `episode/X-Y` - 에피소드 작성 중 (예: `episode/2-2`)
- 작성 완료 후 PR로 main에 머지

## 커밋 메시지 규칙

```
Add episode X-Y: [에피소드 제목]
Update episode X-Y: [수정 내용]
Fix episode X-Y: [버그 수정]
```

## 질문이나 논의

- GitHub Issues 사용
- 라벨: `writing`, `character`, `worldbuilding`, `technical`

## 기여자

- [팀원 이름 추가]

---

**중요**: 작성 전 반드시 `WRITING_GUIDE.md`를 읽어주세요!

# 기여 가이드

**데우스 원정대** 프로젝트에 기여해주셔서 감사합니다!

## 시작하기

### 1. 저장소 클론

```bash
git clone https://github.com/Exiled-germ/deus-expedition.git
cd deus-expedition
```

### 2. 필수 문서 읽기

작성 전 반드시 읽어야 할 문서들:

1. **README.md** - 프로젝트 개요
2. **WRITING_GUIDE.md** ⭐ 가장 중요!
3. **Braindump.md** - 핵심 아이디어
4. **Outline/full-structure.md** - 전체 구조
5. **Characters.md** - 캐릭터 설정
6. **Worldbuilding.md** - 세계관
7. **Style.md** - 문체 가이드

### 3. 작업 흐름

#### 에피소드 작성

1. **작업할 에피소드 선택**
   - `Outline/full-structure.md`에서 확인
   - GitHub Issues에서 "작업 중" 표시

2. **브랜치 생성**
   ```bash
   git checkout -b episode/X-Y
   ```

3. **템플릿 복사**
   ```bash
   cp EPISODE_TEMPLATE.md Chapters/episode-X-Y.md
   ```

4. **작성**
   - `WRITING_GUIDE.md` 참고
   - `Chapters/episode-2-1.md` 예시 참고
   - 분량: 3,500~4,500자 (공백 포함)

5. **자가 검토**
   - `WRITING_GUIDE.md`의 체크리스트 확인
   - 맞춤법 검사
   - 전체 읽어보기

6. **커밋 & 푸시**
   ```bash
   git add Chapters/episode-X-Y.md
   git commit -m "Add episode X-Y: [에피소드 제목]"
   git push origin episode/X-Y
   ```

7. **Pull Request 생성**
   - GitHub에서 PR 생성
   - 템플릿에 따라 작성
   - 리뷰 요청

## 커밋 메시지 규칙

### 형식
```
[타입] [대상]: [간단한 설명]
```

### 타입
- `Add` - 새 에피소드 추가
- `Update` - 기존 에피소드 수정
- `Fix` - 오타나 버그 수정
- `Docs` - 문서 수정
- `Refactor` - 구조 개선

### 예시
```
Add episode 2-2: 먼지 쌓인 검
Update episode 2-1: 리소스 정리 추가
Fix episode 2-1: 오타 수정
Docs: WRITING_GUIDE.md 업데이트
```

## Pull Request 템플릿

PR 생성 시 다음 내용을 포함해주세요:

```markdown
## 에피소드 정보
- 에피소드: X-Y
- 제목: [제목]
- 챕터: X - [챕터 제목]

## 체크리스트
- [ ] WRITING_GUIDE.md 읽음
- [ ] 분량 확인 (3,500~4,500자)
- [ ] 캐릭터 말투 일관성 확인
- [ ] 리소스 정리 완료
- [ ] 맞춤법 검사 완료
- [ ] 전체 읽어보기 완료

## 특이사항
[있다면 작성]

## 리뷰 요청 사항
[특별히 확인받고 싶은 부분]
```

## 코드 리뷰

### 리뷰어 체크리스트

- [ ] 분량 적절 (3,500~4,500자)
- [ ] 형식 준수 (`·` 형식, 헤더 등)
- [ ] A의 목소리 일관성
- [ ] 캐릭터 말투 일관성
- [ ] 전체 스토리 흐름과 일치
- [ ] 리소스 정리 완료
- [ ] 맞춤법 확인

### 리뷰 코멘트 예시

**좋은 코멘트**
```
이 부분 A의 냉소적인 목소리가 잘 드러나네요!
```

**개선 제안**
```
이 대사가 B의 평소 말투와 다른 것 같아요. 
"~습니다" 형식으로 바꾸면 어떨까요?
```

**질문**
```
이 장면에서 A가 이렇게 반응하는 이유가 궁금해요.
이전 에피소드와 연결되는 부분인가요?
```

## 브랜치 전략

### 브랜치 종류

- `main` - 완성되고 리뷰된 에피소드만
- `episode/X-Y` - 에피소드 작성 중
- `docs/[주제]` - 문서 수정
- `fix/[내용]` - 버그 수정

### 브랜치 명명 규칙

```
episode/2-1    # 에피소드 2-1 작성
episode/3-5    # 에피소드 3-5 작성
docs/guide     # 가이드 문서 수정
fix/typo-2-1   # 에피소드 2-1 오타 수정
```

## 이슈 관리

### 이슈 라벨

- `writing` - 에피소드 작성 관련
- `character` - 캐릭터 설정 질문
- `worldbuilding` - 세계관 질문
- `technical` - 기술적 문제
- `discussion` - 논의 필요
- `help wanted` - 도움 요청

### 이슈 템플릿

#### 에피소드 작업 선언
```markdown
## 작업 에피소드
- 에피소드: X-Y
- 제목: [제목]

## 예상 완료일
[날짜]

## 질문사항
[있다면 작성]
```

#### 질문/논의
```markdown
## 질문 내용
[구체적으로 작성]

## 관련 문서
- [관련 파일이나 에피소드]

## 제안
[있다면 작성]
```

## 문서 기여

에피소드 외에도 다음 문서들을 개선할 수 있습니다:

- `README.md` - 프로젝트 소개
- `WRITING_GUIDE.md` - 작성 가이드
- `Characters.md` - 캐릭터 설정
- `Worldbuilding.md` - 세계관
- `Style.md` - 문체 가이드

문서 수정 시:
1. `docs/[주제]` 브랜치 생성
2. 수정 후 PR
3. 팀원 리뷰

## 질문이나 도움이 필요하면

- GitHub Issues에 질문 올리기
- 라벨: `help wanted`, `question`
- 팀원들이 답변해드립니다!

---

**함께 멋진 이야기를 만들어갑시다! 🚀**

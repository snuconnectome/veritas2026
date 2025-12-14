# GitHub 레포지토리 설정 가이드

## 현재 상황
- ✅ 커밋 완료: "Add GitHub Pages website structure and documentation"
- ❌ 푸시 실패: 레포지토리를 찾을 수 없음

## 해결 방법

### 방법 1: GitHub에서 새 레포지토리 생성

1. GitHub.com에 로그인
2. 우측 상단 `+` 클릭 → "New repository"
3. 레포지토리 정보 입력:
   - **Repository name**: `grant_veritas` (또는 원하는 이름)
   - **Visibility**: Public 또는 Private
   - **README, .gitignore, license는 추가하지 않기** (이미 있음)
4. "Create repository" 클릭

### 방법 2: 기존 레포지토리 확인

레포지토리가 이미 있다면:
- URL이 정확한지 확인
- 접근 권한이 있는지 확인
- 레포지토리 이름이 정확한지 확인

## 레포지토리 생성 후 푸시

```bash
cd ~/Desktop/veritas-lecture-2

# 레포지토리가 새로 생성된 경우
git remote set-url origin https://github.com/jcha9928/grant_veritas.git

# 또는 다른 이름으로 생성한 경우
git remote set-url origin https://github.com/jcha9928/새레포지토리이름.git

# 푸시
git push -u origin main
```

## 레포지토리 이름이 다른 경우

```bash
# 원격 레포지토리 URL 변경
git remote set-url origin https://github.com/jcha9928/새로운레포지토리이름.git

# 푸시
git push -u origin main
```

## 현재 커밋된 파일들

다음 파일들이 커밋되어 있습니다:
- ✅ `docs/` - GitHub Pages 홈페이지 전체 구조
- ✅ `CODEBASE_ONBOARDING.md`
- ✅ `GITHUB_PAGES_SETUP.md`
- ✅ `PUSH_INSTRUCTIONS.md`

## 다음 단계

1. GitHub에서 레포지토리 생성 또는 확인
2. 위 명령어로 푸시
3. GitHub Pages 설정 (Settings → Pages → Source: `/docs`)


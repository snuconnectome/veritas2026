# GitHub Pages 활성화 가이드

## ✅ 완료된 작업

- ✅ 레포지토리 생성: `snuconnectome/veritas2026`
- ✅ 모든 파일 푸시 완료
- ✅ 브랜치: `main`

## 🔧 GitHub Pages 활성화

### 방법 1: GitHub 웹사이트에서 설정

1. https://github.com/snuconnectome/veritas2026 접속
2. **Settings** 탭 클릭
3. 왼쪽 메뉴에서 **Pages** 클릭
4. **Source** 섹션에서:
   - Branch: `main` 선택
   - Folder: `/docs` 선택
5. **Save** 클릭

### 방법 2: GitHub CLI로 설정

```bash
cd ~/Desktop/veritas-lecture-2
gh api repos/snuconnectome/veritas2026/pages -X POST -f source[branch]=main -f source[path]=/docs
```

## 🌐 홈페이지 URL

설정 완료 후 몇 분 후 다음 URL에서 확인 가능:
- **https://snuconnectome.github.io/veritas2026**

## 📝 _config.yml 수정 (선택사항)

현재 설정:
```yaml
url: "https://yourusername.github.io"
baseurl: "/veritas-lecture-2"
```

수정 권장:
```yaml
url: "https://snuconnectome.github.io"
baseurl: "/veritas2026"
```

수정 후 다시 푸시:
```bash
cd ~/Desktop/veritas-lecture-2
git add docs/_config.yml
git commit -m "Update GitHub Pages URL configuration"
git push
```

## ✅ 확인 사항

- [ ] GitHub Pages 활성화 완료
- [ ] 홈페이지 접속 확인
- [ ] _config.yml URL 수정 (선택)
- [ ] 모든 섹션이 정상 표시되는지 확인

## 🎉 완료!

홈페이지가 정상적으로 작동하면 베리타스 강좌 2 프로젝트를 공개적으로 공유할 수 있습니다!


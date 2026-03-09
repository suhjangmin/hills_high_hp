# GitHub에 올리는 방법

로컬에서 **이미 해 둔 작업**:
- ✅ `.gitignore` 추가
- ✅ `git init` (저장소 생성)
- ✅ `git add .` (모든 파일 스테이징)
- ✅ `git commit -m "Initial commit: HILLS HIGH LP (HTML/CSS)"` (첫 커밋)

---

## 남은 작업 (직접 하실 부분)

### 1. GitHub에서 새 저장소 만들기

1. **https://github.com/new** 접속 후 로그인
2. **Repository name**: 원하는 이름 입력 (예: `hp`, `hills-high`, `hills-high-lp`)
3. **Public** 선택
4. **"Add a README file"** 등 추가 옵션은 **체크하지 말고** 비워 둠
5. **Create repository** 클릭

---

### 2. 터미널에서 원격 연결 후 푸시

저장소를 만든 뒤 GitHub에 나오는 주소를 사용합니다.  
(예: `https://github.com/당신의아이디/저장소이름.git`)

```bash
cd /Users/jangminsuh/Desktop/hp

# 원격 저장소 연결 (아래 주소를 본인 저장소 주소로 바꾸세요)
git remote add origin https://github.com/당신의아이디/저장소이름.git

# main 브랜치를 GitHub로 푸시
git push -u origin main
```

**GitHub에서 SSH를 쓰는 경우**:
```bash
git remote add origin git@github.com:당신의아이디/저장소이름.git
git push -u origin main
```

---

### 3. (선택) GitHub Pages로 공개하기

1. GitHub 저장소 페이지에서 **Settings** → 왼쪽 메뉴 **Pages**
2. **Build and deployment** → **Source**: **Deploy from a branch**
3. **Branch**: `main` / **Folder**: `/ (root)` 선택 후 **Save**
4. 몇 분 후 `https://당신의아이디.github.io/저장소이름/` 로 접속 가능

---

## 요약

| 단계 | 작업 |
|------|------|
| 1 | GitHub에서 새 저장소 생성 (README 등 추가 없이) |
| 2 | `git remote add origin (저장소URL)` |
| 3 | `git push -u origin main` |
| 4 | (선택) Settings → Pages 에서 배포 설정 |

이후 수정 사항이 있으면:
```bash
git add .
git commit -m "메시지"
git push
```
으로 올리시면 됩니다.

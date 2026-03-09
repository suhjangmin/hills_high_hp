# 무료 호스팅 배포 방법

이 폴더를 **무료**로 인터넷에 공개하는 방법입니다. 아래 중 하나만 하면 됩니다.

---

## 방법 1: Netlify Drop (가장 간단, 가입만 하면 됨)

1. 브라우저에서 **https://app.netlify.com/drop** 접속
2. Netlify 계정으로 로그인(또는 무료 가입)
3. **이 폴더 전체(`hp`)** 를 드래그해서 화면에 놓기
4. 잠시 후 `https://랜덤이름.netlify.app` 형태의 URL이 생성됨 → 이 주소로 누구나 접속 가능

---

## 방법 2: Vercel (Node.js 설치된 경우)

터미널에서:

```bash
cd /Users/jangminsuh/Desktop/hp
npx vercel --yes
```

처음이면 로그인 안내가 나오면 따라 하고, 다시 위 명령 실행.  
완료 후 터미널에 나온 `https://프로젝트이름.vercel.app` 주소로 접속하면 됩니다.

---

## 방법 3: GitHub Pages

1. **GitHub**에서 새 저장소 만들기 (이름 예: `hp` 또는 `hills-high`)
2. 터미널에서:

```bash
cd /Users/jangminsuh/Desktop/hp
git init
git add .
git commit -m "Initial: static site"
git branch -M main
git remote add origin https://github.com/당신의아이디/저장소이름.git
git push -u origin main
```

3. GitHub 저장소 **Settings → Pages** 로 이동  
   - Source: **Deploy from a branch**  
   - Branch: **main**  
   - Folder: **/ (root)**  
   - Save
4. 몇 분 후 `https://당신의아이디.github.io/저장소이름/` 로 접속 가능

---

## 방법 4: Cloudflare Pages

1. **https://dash.cloudflare.com** 로그인 후 **Workers & Pages** → **Create** → **Pages** → **Connect to Git** 또는 **Upload assets**
2. **Upload assets** 선택 시 이 폴더를 zip으로 압축한 뒤 업로드
3. 배포 완료 후 `https://프로젝트이름.pages.dev` 형태의 URL로 접속

---

원하시면 **방법 1 (Netlify Drop)** 만 따라 하시면 됩니다.  
폴더만 끌어다 놓으면 되고, URL은 자동으로 부여됩니다.

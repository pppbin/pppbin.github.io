# 이력서 사이트 (Jekyll)

## 1. 내용 수정하기
- `_config.yml` : 사이트 제목, 이름, 이메일, GitHub 아이디 수정
- `index.html` : 경력, 학력, 기술 스택, 프로젝트 내용을 본인 정보로 교체
- `assets/css/style.css` : 색상 등 디자인 변경 (선택)

## 2. GitHub Pages에 올리기

1. GitHub에서 새 저장소 생성
   - 개인 프로필 사이트로 만들려면 저장소 이름을 `your-github-id.github.io` 로 지정
   - 별도 프로젝트 사이트로 만들려면 아무 이름이나 사용 가능
2. 이 폴더의 파일들을 저장소에 push:
   ```bash
   git init
   git add .
   git commit -m "이력서 사이트 초기 생성"
   git branch -M main
   git remote add origin https://github.com/your-github-id/your-repo.git
   git push -u origin main
   ```
3. 저장소 이름을 `your-github-id.github.io`로 만들었다면 자동으로
   `https://your-github-id.github.io` 에서 바로 확인 가능합니다.
4. 다른 이름의 저장소라면 GitHub 저장소 > Settings > Pages 에서
   Source를 "Deploy from a branch" → `main` 브랜치로 설정하면
   `https://your-github-id.github.io/저장소이름` 에서 확인 가능합니다.
   (반영까지 1~2분 정도 걸릴 수 있어요)

## 3. 로컬에서 미리보기 (선택)
Ruby와 Bundler가 설치되어 있다면:
```bash
bundle install
bundle exec jekyll serve
```
그 후 `http://localhost:4000` 접속.

### 프로젝트 개발 과정

1. Ruby, Jekyll을 활용한 기초 html 사이트 개설
 - 정적 웹사이트를 개설하기 위해 Ruby, Jekyll를 설치받고 Github에서
   새로운 Repo를 만들어 개발환경을 구축한뒤에 bundle과로 홈페이지를 활성화 한뒤
   theme나 _config.yml를 수정하여 나의 입맛대로 홈페이지를 꾸밀수 있게 만든다.
   또한 홈페이지를 호스팅 해주는 Disqus를 사용하여 Github와 연동하여 자동 업데이트가 되게 만들었다.

2. 중요 명령들
```dash
cd <mydirectory>
git clone https://github.com/<username>/<username>.github.io.git
jekyll new . --force
bundle exec jekyll serve
```
_config.yml 수정후

```dash
git rm index.html
git add *
git commit
git push origin main
```

_post, 테마 적용 후
_layouts/post.html 수정
PAGE_URL과 PAGE_IDENTIFIER에 Disqus 정보입력

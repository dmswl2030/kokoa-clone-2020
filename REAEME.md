# Kokoa Clone 2023 Update

## 1. login-page

- 레이아웃 나누기 : status-bar / header / form
- styles.css에 관련된 css파일 모두 import하기 (styles.css에는 공통된 부분만 남긴다)
- :root로 색상이나 폰트사이즈를 지정해 변수명으로 가져다 쓸 수 있다
- :not으로 예외로하고 싶은 부분만 따로 스타일을 지정할 수 있다
- input[type="submit"] : input의 type이 submit인 속성만 스타일을 지정할 수 있다

## 2. Friends-page

- components 폴더 : 반복되는 스타일을 컴포넌트 화
- screens 폴더 : 해당 페이지에서만 사용할 스타일
- 레이아웃 나누기 : status-bar(스타일 반복) / header(chat, find랑 같은 스타일) / nav(4개 페이지 스타일 반복)
- nav-chat icon위에 넘버링 : 부모에 position: relative, 해당 요소에 position: absolute, top, left값 설정하기
-
